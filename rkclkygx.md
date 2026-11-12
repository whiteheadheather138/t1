代发 wailian999

================================================================================
来源：http://zty.smart0.xyz

G. 面向对象
来源：http://lcn.yueranfly.top

================================================================================
来源：http://pdj.hfpthk.cn

[G01] 定义类
来源：http://qdc.iojbl.cn

Py:   class User: pass
来源：http://fce.fengsongda.top

PHP:  class User {}
来源：http://dal.redwolf501.top

JS:   class User {}
来源：http://ldu.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://fbg.smart0.xyz

Java: class User {}
来源：http://vnf.cdnleiting.top

Go:   type User struct { Name string }
来源：http://clf.yj202588.top

Ruby: class User; end
来源：http://tdg.yj202588.top

C#:   class User {}
来源：http://xvb.nanxinkj.top

[G02] 构造函数
来源：http://pvf.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://hes.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://vht.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ejw.meibo888.top

TS:   constructor(public name: string) {}
来源：http://eck.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://srr.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sdr.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ymw.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://etu.xylfe.cn

[G03] 实例属性
来源：http://rze.aibaodan.cn

Py:   self.name = "x"
来源：http://lih.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://pnz.gotoacloud.top

JS:   this.name = "x";
来源：http://dit.zdbjq.cn

TS:   name: string = "x";
来源：http://thp.sxryk.cn

Java: private String name;
来源：http://mdu.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://evn.xinyue.icu

Ruby: @name = "x"
来源：http://gfs.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://qet.guannengcc.top

[G04] 定义方法
来源：http://jhf.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://ukm.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qxq.sweek.top

JS:   greet() { return this.name; }
来源：http://exy.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://gnt.yvedp.cn

Java: String greet() { return name; }
来源：http://dhn.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gqg.xziqi.cn

Ruby: def greet; @name; end
来源：http://ndd.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://fzh.feifeiyinyue.top

[G05] 继承
来源：http://nrv.fehbvm.com

Py:   class Admin(User): pass
来源：http://jdh.hesvh.cn

PHP:  class Admin extends User {}
来源：http://grq.ctjpmb.com

JS:   class Admin extends User {}
来源：http://lop.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://lwk.yj20258.top

Java: class Admin extends User {}
来源：http://lqg.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ccm.yj202588.top

Ruby: class Admin < User; end
来源：http://fyh.jinqigufen.top

C#:   class Admin : User {}
来源：http://unu.chenzaomai.com

[G06] 重写方法
来源：http://bss.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://wli.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qho.zhengqikj.top

JS:   greet() { return "admin"; }
来源：http://fev.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://krl.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://icj.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vqa.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://dyi.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://ssk.wangshuangyany.cn

[G07] 调用父类方法
来源：http://phz.mhx1999.top

Py:   super().greet()
来源：http://kbn.xziqi.cn

PHP:  parent::greet();
来源：http://yrk.9152youxi.cn

JS:   super.greet();
来源：http://lku.yonumen.top

TS:   super.greet();
来源：http://ceq.jinqigfzy.top

Java: super.greet();
来源：http://cva.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dct.tian-w.cn

Ruby: super
来源：http://kma.hnqzz.top

C#:   base.Greet();
来源：http://zmc.zhijiandao.cn

[G08] 静态方法与属性
来源：http://gzw.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ftm.meibo888.top

PHP:  public static function f() {}
来源：http://cad.zhijiandao.cn

JS:   static f() {}
来源：http://ung.pycfn.com

TS:   static f(): void {}
来源：http://mfr.yj20258.top

Java: static void f() {}
来源：http://ybi.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rnv.xinyue.icu

Ruby: def self.f; end
来源：http://gin.haohaochexian.top

C#:   public static void F() {}
来源：http://glg.fehbvm.com

[G09] 接口 / 抽象类
来源：http://vcz.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://pwj.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://aiz.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dva.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://yex.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://bgv.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://bnj.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zsc.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://iyz.havefunace.top

[G10] 访问控制
来源：http://kma.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://stn.jyoumei.cn

PHP:  public / protected / private
来源：http://zzd.tarul.cn

JS:   #private 字段；其余公开
来源：http://zts.xuanzx.com

TS:   public / protected / private
来源：http://vdc.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://smf.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gug.vehdjk.com

Ruby: public / protected / private
来源：http://quq.yonumen.top

C#:   public / protected / private / internal
来源：http://nsz.chenzaomai.com

[G11] getter / setter
来源：http://avz.iojbl.cn

Py:   @property 与 @x.setter
来源：http://end.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wjo.daria6918.cn

JS:   get name() { return this._name; }
来源：http://pgu.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://ptv.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://lrn.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://riy.meibo888.top

Ruby: attr_accessor :name
来源：http://yxz.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://fmn.yj20258888.top

[G12] 对象转字符串
来源：http://rds.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://vrn.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fgx.fengsongda.top

JS:   toString() { return this.name; }
来源：http://tmd.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://vax.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://sfx.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mnj.fehbvm.com

Ruby: def to_s; @name; end
来源：http://zxi.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://mds.ehwqpu.com

[G13] 判断对象类型
来源：http://tsg.bjfxy.top

Py:   isinstance(u, User)
来源：http://bvl.daxiang520.top

PHP:  $u instanceof User
来源：http://dbf.chenlongwang.top

JS:   u instanceof User
来源：http://bhr.jiagoushi.top

TS:   u instanceof User
来源：http://uec.tanke756.top

Java: u instanceof User
来源：http://jfm.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eqf.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://pda.hywenlv.cn

C#:   u is User
来源：http://imo.sysykeji.top

[G14] 数据类 / record
来源：http://crn.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zde.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://bdi.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aba.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://pgv.hammf.cn

Java: record User(String name, int age) {}
来源：http://fdy.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://sbn.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://feg.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://rfq.hfpthk.cn

[G15] 枚举
来源：http://pnp.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xgd.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hth.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jza.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ivc.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://iok.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pnr.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://ivg.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jjs.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://gyq.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tpd.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://elb.sxryk.cn

JS:   Object.entries(obj)
来源：http://ryi.cucudq.cn

TS:   Object.entries(obj)
来源：http://aom.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://msa.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zmt.xziqi.cn

Ruby: obj.instance_variables
来源：http://vua.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://zeu.xuetiantiany.cn

================================================================================
来源：http://fmd.cashguo.top

H. 异常与错误处理
来源：http://ria.sjlbkw.cn

================================================================================
来源：http://sgw.tian-w.cn

[H01] try / catch 基础
来源：http://snv.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rhj.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zat.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qil.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://joe.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zdu.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://swj.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dkl.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zst.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://thi.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://mzu.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lpi.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://bcl.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nuo.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://rnv.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tfp.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ztm.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vcm.havefunace.top

[H03] 主动抛出异常
来源：http://jev.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://wvp.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pvr.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://qyt.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://gae.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wla.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://art.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://oys.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://mqy.yonumen.top

[H04] 自定义异常类型
来源：http://aii.zhiwuduotai.top

Py:   class MyError(Exception): pass
来源：http://npt.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://idw.vehdjk.com

JS:   class MyError extends Error {}
来源：http://qno.ybcxt.top

TS:   class MyError extends Error {}
来源：http://vpg.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://gwq.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lqq.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://gam.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://oez.epnwcf.com

[H05] 捕获特定类型
来源：http://apb.zhengqikj.top

Py:   except ValueError as e:
来源：http://lvt.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sgs.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://iqg.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://mss.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://sih.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qwi.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://jgz.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://smp.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://xdp.kuanghao11.cn

Py:   value = d.get("k") or default
来源：http://eyh.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://egs.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ijv.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://cwo.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nbh.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bkm.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://wzw.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://fhy.nanxuanxn.top

[H07] 断言
来源：http://kco.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://mbe.bjfxy.top

PHP:  assert($x > 0);
来源：http://gtg.yangfankeji.com

JS:   console.assert(x > 0);
来源：http://wjm.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://yqx.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://ghx.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uag.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://qvf.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://ufb.sweek.top

[H08] 获取错误信息与堆栈
来源：http://unv.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://lss.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yae.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://fef.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wjp.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bwc.hnqzz.top

Go:   err.Error()
来源：http://jut.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://jta.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://loz.meibo888.top

[H09] 带错误码的异常
来源：http://zeq.jqgfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jrb.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gon.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aps.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lqr.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dwb.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://awv.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qdb.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hiw.aibaodan.cn

[H10] 资源自动释放
来源：http://cxt.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://bfj.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ivo.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tia.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czf.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dyk.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://jej.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lyd.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cez.kuanghao11.cn

================================================================================
来源：http://ezw.aizwys.cn

I. 正则表达式
来源：http://wiy.yj20258888.top

================================================================================
来源：http://zbk.sweek.top

[I01] 判断是否匹配
来源：http://fwd.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yer.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://vtv.andypj.xyz

JS:   /\d+/.test(s)
来源：http://ycs.epnwcf.com

TS:   /\d+/.test(s)
来源：http://zty.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tqn.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://thf.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://cfl.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zlf.nanxuanxn.top

[I02] 提取所有匹配
来源：http://kkl.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://hdr.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kas.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rpu.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://nzv.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fsq.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://udq.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://qqn.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://prl.jianghu66.top

[I03] 提取捕获分组
来源：http://ozo.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ysx.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fts.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iyg.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://grb.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dex.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jmy.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybm.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aky.316326.xyz

[I04] 正则替换
来源：http://idj.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://tbn.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://owt.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://fsn.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://fwv.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://qag.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hqy.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fnz.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xlw.wangdashe.top

[I05] 按正则拆分
来源：http://rlm.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mvd.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tle.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://lgl.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://zmr.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://ayz.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://epg.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://uuj.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zkz.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://epd.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ewr.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ufd.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cst.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ytm.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tsi.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xxs.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nax.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dzf.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://yxj.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qdi.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vti.meibo888.top


<!-- 参考信息 -->