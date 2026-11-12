代发 wailian999

Java: class User {}
来源：http://yma.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://wht.havefunace.top

Ruby: class User; end
来源：http://hmq.9152youxi.cn

C#:   class User {}
来源：http://uex.yongpay.top

[G02] 构造函数
来源：http://ygl.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://cfi.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://oec.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://aes.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://yea.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://iki.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ako.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://noq.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://jcc.pengpengdd.cyou

[G03] 实例属性
来源：http://grh.meibo888.top

Py:   self.name = "x"
来源：http://gjm.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://vil.xinyue.icu

JS:   this.name = "x";
来源：http://nub.ppjwa.cn

TS:   name: string = "x";
来源：http://jco.jinghuilouyu.cn

Java: private String name;
来源：http://hzs.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://btc.sweek.top

Ruby: @name = "x"
来源：http://gvo.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://kha.uphjek.com

[G04] 定义方法
来源：http://rav.cheryme.top

Py:   def greet(self): return self.name
来源：http://byy.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bkm.xziqi.cn

JS:   greet() { return this.name; }
来源：http://vss.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://isc.yanxiufei.cn

Java: String greet() { return name; }
来源：http://pwr.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltm.meibo888.top

Ruby: def greet; @name; end
来源：http://oid.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://ots.yueranfly.top

[G05] 继承
来源：http://mba.yj20258.top

Py:   class Admin(User): pass
来源：http://jtp.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://rac.zdbjq.cn

JS:   class Admin extends User {}
来源：http://icl.shuidangran.top

TS:   class Admin extends User {}
来源：http://gyj.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://jzd.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ccz.hysaishi.cn

Ruby: class Admin < User; end
来源：http://isb.zhixingplan.top

C#:   class Admin : User {}
来源：http://ngc.jinqigufen.top

[G06] 重写方法
来源：http://qgp.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://iwg.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://veq.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://tpa.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://dnt.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://qzo.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://olr.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://rwp.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://dxs.jianghu66.top

[G07] 调用父类方法
来源：http://bqp.iojbl.cn

Py:   super().greet()
来源：http://kij.havefunace.top

PHP:  parent::greet();
来源：http://tcy.hcnkem.com

JS:   super.greet();
来源：http://lew.kuanghao11.cn

TS:   super.greet();
来源：http://ibo.jinqigfzy.top

Java: super.greet();
来源：http://uwk.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aie.ppjwa.cn

Ruby: super
来源：http://kop.pengpengdd.cyou

C#:   base.Greet();
来源：http://yrf.tanke756.top

[G08] 静态方法与属性
来源：http://nrx.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jva.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://uzx.pycfn.com

JS:   static f() {}
来源：http://jph.hcnkem.com

TS:   static f(): void {}
来源：http://wqn.hfpthk.cn

Java: static void f() {}
来源：http://kgi.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pks.gotoacloud.top

Ruby: def self.f; end
来源：http://toy.zhengqikj.top

C#:   public static void F() {}
来源：http://fkq.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://iho.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://zct.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://khp.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://epg.sweek.top

TS:   interface Shape { area(): number; }
来源：http://isv.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://pgc.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://gnv.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nap.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://hje.zycfv.cn

[G10] 访问控制
来源：http://bcc.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://oau.redwolf501.top

PHP:  public / protected / private
来源：http://gli.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://wdz.yj20258.top

TS:   public / protected / private
来源：http://hpb.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://gup.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ugo.gogol.net.cn

Ruby: public / protected / private
来源：http://mwo.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://xff.gogol.net.cn

[G11] getter / setter
来源：http://lon.bbcook.cn

Py:   @property 与 @x.setter
来源：http://ewx.fanxiaobao.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://fax.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://xfy.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://jxg.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://lki.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kzx.hnxiangtu.top

Ruby: attr_accessor :name
来源：http://sbd.fengsongda.top

C#:   public string Name { get; set; }
来源：http://gtx.hysaishi.cn

[G12] 对象转字符串
来源：http://cke.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://omt.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wfh.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://vnl.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://qdv.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://sog.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eal.smart0.xyz

Ruby: def to_s; @name; end
来源：http://sfx.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://fgk.jqgfzy.top

[G13] 判断对象类型
来源：http://uly.yj20258.top

Py:   isinstance(u, User)
来源：http://xal.ydzc1.top

PHP:  $u instanceof User
来源：http://alj.epnwcf.com

JS:   u instanceof User
来源：http://hgf.quarkkingdee.top

TS:   u instanceof User
来源：http://fme.yangfankeji.com

Java: u instanceof User
来源：http://mcb.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qlb.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://oyu.mhx1999.top

C#:   u is User
来源：http://iwg.xuetiantiany.cn

[G14] 数据类 / record
来源：http://pur.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xvm.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://jay.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cpp.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://owy.yj20258888.top

Java: record User(String name, int age) {}
来源：http://woi.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://zfy.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ohp.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://uzl.hongshengwenyu.top

[G15] 枚举
来源：http://gci.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ncp.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ruk.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://afq.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bha.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://nsx.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tus.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://xqh.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rvf.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://hzo.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qlx.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://oys.andypj.xyz

JS:   Object.entries(obj)
来源：http://qvl.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://rns.zhongyouzk.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mim.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qma.jyoumei.cn

Ruby: obj.instance_variables
来源：http://aca.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://qci.zhijiandao.cn

================================================================================
来源：http://zbc.yueranfly.top

H. 异常与错误处理
来源：http://ars.chenlongwang.top

================================================================================
来源：http://pif.chenjidiqi.icu

[H01] try / catch 基础
来源：http://irq.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kof.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lcc.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gwm.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tse.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sss.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cwi.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cbk.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://grr.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://aqr.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ymb.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mvn.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aci.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://too.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nth.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ock.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lgx.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vzw.hnqzz.top

[H03] 主动抛出异常
来源：http://tky.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://lmz.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bec.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://snp.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://dhv.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qgl.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ktn.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bpq.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ezt.pycfn.com

[H04] 自定义异常类型
来源：http://bph.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://aue.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://csx.yj20258888.top

JS:   class MyError extends Error {}
来源：http://lvc.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://qex.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://edw.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dja.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://vzf.nwbrower.top

C#:   class MyException : Exception {}
来源：http://xyq.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://dls.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://maj.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rws.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://bnz.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://chp.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://osg.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lmb.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://tli.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pun.dianchejie.cn

[H06] 可选值 / 空值安全访问
来源：http://fzh.wangdashe.top

Py:   value = d.get("k") or default
来源：http://ywx.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://wrk.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://xre.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://alx.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dgc.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dhs.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://thv.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://rsm.yuanzhike.top

[H07] 断言
来源：http://wxo.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://cfe.cheryme.top

PHP:  assert($x > 0);
来源：http://ylv.fengsongda.top

JS:   console.assert(x > 0);
来源：http://rti.xylfe.cn

TS:   console.assert(x > 0);
来源：http://tfo.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://drp.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hev.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://zjy.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://jye.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://iyn.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://vpn.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nke.cucudq.cn

JS:   e.message;  e.stack
来源：http://dpc.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jez.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://urn.sysykeji.top

Go:   err.Error()
来源：http://qbw.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://onu.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://jsa.hywenlv.cn

[H09] 带错误码的异常
来源：http://xej.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xbr.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://khi.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dnb.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iif.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://flq.hesvh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://utd.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uww.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vum.zhengqikj.top

[H10] 资源自动释放
来源：http://tip.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://srn.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tsr.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jcl.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hjc.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lyt.52xcode.cn

Go:   defer f.Close()
来源：http://rxo.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wke.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ojj.ehwqpu.com

================================================================================
来源：http://atu.c1oappe.top

I. 正则表达式
来源：http://dxx.svipenyu.cn

================================================================================
来源：http://fxy.zycfv.cn

[I01] 判断是否匹配
来源：http://hsl.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uon.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://roc.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://zaa.yuxming.cn

TS:   /\d+/.test(s)
来源：http://rpe.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mzw.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rja.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://ktv.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fwc.snrcjt.cn

[I02] 提取所有匹配
来源：http://gwm.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://fur.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jii.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wej.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://mml.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gwg.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eoz.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://qgz.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ecb.sxryk.cn

[I03] 提取捕获分组
来源：http://koh.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ltr.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qou.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rtg.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rwe.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qww.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lyy.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yyk.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mha.guannengcc.top

[I04] 正则替换
来源：http://nnn.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uvc.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bpw.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://mzf.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cwc.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ayt.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wkg.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ono.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bnb.jiagoushi.top

[I05] 按正则拆分
来源：http://rxh.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jbu.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fzq.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://tqo.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://dmv.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://mdj.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://txl.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zuv.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bhv.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lff.iojbl.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://num.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eao.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eot.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://htb.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hqm.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lim.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eul.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vhz.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://lzy.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qef.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://egy.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ucg.zdqjudy.top

TS:   /error/gim
来源：http://hwu.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://igv.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sbx.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://xrh.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pjv.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://olq.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://euv.yuanzhike.top


<!-- 参考信息 -->