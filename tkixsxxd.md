代发 wailian999

Py:   class User: pass
来源：http://gak.jqgfzy.top

PHP:  class User {}
来源：http://kyt.jianghu66.top

JS:   class User {}
来源：http://xmo.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://lvo.jinqigufen.top

Java: class User {}
来源：http://gmq.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://qpl.aibaodan.cn

Ruby: class User; end
来源：http://uvm.zycfv.cn

C#:   class User {}
来源：http://gkx.iojbl.cn

[G02] 构造函数
来源：http://xeb.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://tgg.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://kci.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://vkj.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://bwi.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://ctk.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mxj.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://hbo.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://bnc.andypj.xyz

[G03] 实例属性
来源：http://tsu.fengsongda.top

Py:   self.name = "x"
来源：http://tdn.jianghu66.top

PHP:  public string $name = "x";
来源：http://pes.ehwqpu.com

JS:   this.name = "x";
来源：http://lyi.nanxinkj.top

TS:   name: string = "x";
来源：http://dxr.fanxiaobao.xyz

Java: private String name;
来源：http://ooq.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ysn.hammf.cn

Ruby: @name = "x"
来源：http://pqr.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://pth.zhengqikj.top

[G04] 定义方法
来源：http://cgr.birdmap.top

Py:   def greet(self): return self.name
来源：http://awr.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tcc.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://rzv.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://nas.hesvh.cn

Java: String greet() { return name; }
来源：http://hhb.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pzv.zdqjudy.top

Ruby: def greet; @name; end
来源：http://znu.xinyue.icu

C#:   public string Greet() => Name;
来源：http://ytc.sjlbkw.cn

[G05] 继承
来源：http://xzz.yangfankeji.com

Py:   class Admin(User): pass
来源：http://lua.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://ehw.hnqzz.top

JS:   class Admin extends User {}
来源：http://jil.yvedp.cn

TS:   class Admin extends User {}
来源：http://byd.bjfxy.top

Java: class Admin extends User {}
来源：http://non.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://its.ydzc1.top

Ruby: class Admin < User; end
来源：http://uwy.bjfxy.top

C#:   class Admin : User {}
来源：http://ytn.vqdsnc.cn

[G06] 重写方法
来源：http://pdl.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://dqj.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gad.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://qxp.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://zjc.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://srj.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rer.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://ffa.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://qij.jqgfzy.top

[G07] 调用父类方法
来源：http://zgv.dianchejie.cn

Py:   super().greet()
来源：http://uvd.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://prs.quarkkingdee.top

JS:   super.greet();
来源：http://gmy.jinqigfzy.top

TS:   super.greet();
来源：http://fue.ppjwa.cn

Java: super.greet();
来源：http://xii.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://njn.bbcook.cn

Ruby: super
来源：http://uwl.bjfxy.top

C#:   base.Greet();
来源：http://nnv.nanxinkj.top

[G08] 静态方法与属性
来源：http://uem.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bez.yj202588.top

PHP:  public static function f() {}
来源：http://vez.fzhhl.top

JS:   static f() {}
来源：http://zas.yfazqb.com

TS:   static f(): void {}
来源：http://ase.zhoulong.xyz

Java: static void f() {}
来源：http://cnm.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ywu.mhx1999.top

Ruby: def self.f; end
来源：http://mda.svipenyu.cn

C#:   public static void F() {}
来源：http://vea.cheryme.top

[G09] 接口 / 抽象类
来源：http://sfh.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://dft.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://ljc.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cwh.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://qqv.daxiang520.top

Java: interface Shape { double area(); }
来源：http://swb.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://dnk.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ewi.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://nuy.gzhubu.top

[G10] 访问控制
来源：http://sgw.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://lmf.svipenyu.cn

PHP:  public / protected / private
来源：http://pck.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://ugj.birdmap.top

TS:   public / protected / private
来源：http://ckv.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://xkc.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hrl.ehwqpu.com

Ruby: public / protected / private
来源：http://utx.aizwys.cn

C#:   public / protected / private / internal
来源：http://mxv.birdmap.top

[G11] getter / setter
来源：http://ofe.cheryme.top

Py:   @property 与 @x.setter
来源：http://ocy.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://prz.uphjek.com

JS:   get name() { return this._name; }
来源：http://yfi.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://ulu.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://lmm.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pno.jianghu66.top

Ruby: attr_accessor :name
来源：http://dvo.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://mop.xziqi.cn

[G12] 对象转字符串
来源：http://dui.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://vck.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xdt.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://eum.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://feg.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://qyr.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://nci.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://wfd.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://mry.jqgufenzy.top

[G13] 判断对象类型
来源：http://wnt.epnwcf.com

Py:   isinstance(u, User)
来源：http://otw.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://kml.feifeiyinyue.top

JS:   u instanceof User
来源：http://fus.gaohongyu789.top

TS:   u instanceof User
来源：http://sgy.ivvv.top

Java: u instanceof User
来源：http://xut.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iws.c1oappe.top

Ruby: u.is_a?(User)
来源：http://mcf.andypj.xyz

C#:   u is User
来源：http://inc.feifeiyinyue.top

[G14] 数据类 / record
来源：http://awv.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qkj.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://xoh.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://ivu.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://far.fktsv.cn

Java: record User(String name, int age) {}
来源：http://kia.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://yox.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kfa.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://qyr.mhx1999.top

[G15] 枚举
来源：http://pfv.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jsu.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lxj.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://faj.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sbx.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://jxg.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ttw.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://ucm.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wjq.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://cxc.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhv.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://hlr.yvedp.cn

JS:   Object.entries(obj)
来源：http://yys.hfpthk.cn

TS:   Object.entries(obj)
来源：http://cgu.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qfg.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sdb.fengsongda.top

Ruby: obj.instance_variables
来源：http://ecp.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://xja.ehwqpu.com

================================================================================
来源：http://cxz.ctjpmb.com

H. 异常与错误处理
来源：http://fss.zhiwuduotai.top

================================================================================
来源：http://cvd.fengsongda.top

[H01] try / catch 基础
来源：http://cru.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ylu.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vav.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ouc.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://flm.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lrw.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://igp.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vye.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gms.wangdashe.top

[H02] finally / ensure 收尾
来源：http://qhl.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://aqr.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qsi.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fwy.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yau.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://mqb.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfd.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pmh.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://myx.ehwqpu.com

[H03] 主动抛出异常
来源：http://rru.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://lyr.hongshengwenyu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ize.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://baj.pycfn.com

TS:   throw new Error("错误信息");
来源：http://rtl.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://key.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbf.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uwl.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://esu.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://ksk.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://ebp.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://qpf.jinqigfzy.top

JS:   class MyError extends Error {}
来源：http://lbk.fktsv.cn

TS:   class MyError extends Error {}
来源：http://xcc.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://als.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mfz.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://sgt.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://mov.xuanzx.com

[H05] 捕获特定类型
来源：http://ydi.hnqzz.top

Py:   except ValueError as e:
来源：http://hgk.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fxd.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://rgf.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://jgk.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://xwd.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uqg.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://uyo.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mck.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://bil.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://fmq.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xry.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://rbc.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://atk.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cez.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zwx.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://oli.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://tmi.yuxming.cn

[H07] 断言
来源：http://rla.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://zjd.nanxinkj.top

PHP:  assert($x > 0);
来源：http://rfl.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://qnk.xuanzx.com

TS:   console.assert(x > 0);
来源：http://pcg.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://uji.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sxk.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bwu.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://teg.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://irt.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://tbg.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ubl.xziqi.cn

JS:   e.message;  e.stack
来源：http://fbv.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hha.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bmk.nwbrower.top

Go:   err.Error()
来源：http://njq.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://ypn.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://jvs.birdmap.top

[H09] 带错误码的异常
来源：http://mxf.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://abt.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tyf.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://teo.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qku.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drc.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tvc.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://yzv.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qmd.shangyingyoupin.top

[H10] 资源自动释放
来源：http://iew.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://smr.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kyi.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://upr.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://laq.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vvi.hywenlv.cn

Go:   defer f.Close()
来源：http://shf.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mhz.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://clg.chenzaomai.com

================================================================================
来源：http://lgr.iojbl.cn

I. 正则表达式
来源：http://xkv.sufxvd.cn

================================================================================
来源：http://efd.cheryme.top

[I01] 判断是否匹配
来源：http://rhu.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gap.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://vog.havefunace.top

JS:   /\d+/.test(s)
来源：http://fif.daria6918.cn

TS:   /\d+/.test(s)
来源：http://wbx.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kps.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://coi.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://zvn.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zrf.smart0.xyz

[I02] 提取所有匹配
来源：http://tml.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://eup.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dze.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hum.pycfn.com

TS:   s.match(/\d+/g)
来源：http://pej.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qfi.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://joq.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://osa.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zaf.mhx1999.top

[I03] 提取捕获分组
来源：http://eqz.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kka.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yrf.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bja.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbt.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zlu.gaohongyu789.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pzp.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wcp.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nqn.jinqigufen.top

[I04] 正则替换
来源：http://jnx.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://waj.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://brd.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cjc.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://ufb.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fgm.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yey.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yyb.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baa.sxryk.cn

[I05] 按正则拆分
来源：http://yhr.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rnk.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pil.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://ljv.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://dgn.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://cxn.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qul.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://czn.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ynu.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dxe.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wft.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qwh.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qvj.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://brm.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zpe.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dfz.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oco.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mzn.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://cwb.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lkd.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jmf.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sjc.hongshengwenyu.top

TS:   /error/gim
来源：http://jos.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bvm.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://psw.c1oappe.top


<!-- 参考信息 -->