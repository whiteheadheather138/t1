代发 wailian999

[G02] 构造函数
来源：http://pkj.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://vul.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://toj.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://abp.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://dch.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://yas.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://evn.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://bvx.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://xsk.sufxvd.cn

[G03] 实例属性
来源：http://zbo.iojbl.cn

Py:   self.name = "x"
来源：http://tme.daria6918.cn

PHP:  public string $name = "x";
来源：http://hvi.yanxiufei.cn

JS:   this.name = "x";
来源：http://kwv.yj202588.top

TS:   name: string = "x";
来源：http://gyu.daria6918.cn

Java: private String name;
来源：http://qbw.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hvy.meibo888.top

Ruby: @name = "x"
来源：http://rgm.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://liq.hcnkem.com

[G04] 定义方法
来源：http://cah.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://hmn.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pge.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://ivv.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://rik.snrcjt.cn

Java: String greet() { return name; }
来源：http://ymr.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyk.xuanzx.com

Ruby: def greet; @name; end
来源：http://dwp.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://wcg.daxiang520.top

[G05] 继承
来源：http://syy.jianghu66.top

Py:   class Admin(User): pass
来源：http://kqp.shuidangran.top

PHP:  class Admin extends User {}
来源：http://nsi.yuxming.cn

JS:   class Admin extends User {}
来源：http://qvb.bbcook.cn

TS:   class Admin extends User {}
来源：http://kga.cheryme.top

Java: class Admin extends User {}
来源：http://mgo.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uhf.yueranfly.top

Ruby: class Admin < User; end
来源：http://mes.jqgufenzy.top

C#:   class Admin : User {}
来源：http://qul.shanyushiyangkeji.top

[G06] 重写方法
来源：http://fel.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://nzx.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vff.pycfn.com

JS:   greet() { return "admin"; }
来源：http://zpl.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://hfe.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://mmb.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nac.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://tgl.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://euu.nanxinkj.top

[G07] 调用父类方法
来源：http://nuu.havefunace.top

Py:   super().greet()
来源：http://fuz.jqgufenzy.top

PHP:  parent::greet();
来源：http://cgb.pycfn.com

JS:   super.greet();
来源：http://pwa.bbcook.cn

TS:   super.greet();
来源：http://fci.meibo888.top

Java: super.greet();
来源：http://nzv.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wrk.guowangkeji.top

Ruby: super
来源：http://pmd.yongpay.top

C#:   base.Greet();
来源：http://sea.ivvv.top

[G08] 静态方法与属性
来源：http://odm.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qth.yfazqb.com

PHP:  public static function f() {}
来源：http://bzr.gogol.net.cn

JS:   static f() {}
来源：http://emb.jyoumei.cn

TS:   static f(): void {}
来源：http://dna.vehdjk.com

Java: static void f() {}
来源：http://nld.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vyf.hammf.cn

Ruby: def self.f; end
来源：http://pxt.cdnleiting.top

C#:   public static void F() {}
来源：http://gml.xylfe.cn

[G09] 接口 / 抽象类
来源：http://qkc.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://etz.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vmw.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://dag.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://dmm.pycfn.com

Java: interface Shape { double area(); }
来源：http://uhd.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://jaw.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rbb.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://ivk.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://zzh.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://lzh.nanxinkj.top

PHP:  public / protected / private
来源：http://vdz.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://sgw.sjlbkw.cn

TS:   public / protected / private
来源：http://xnz.pycfn.com

Java: public / protected / private / 默认包级
来源：http://wby.cashguo.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uoc.316326.xyz

Ruby: public / protected / private
来源：http://yxp.vehdjk.com

C#:   public / protected / private / internal
来源：http://xhy.zhijiandao.cn

[G11] getter / setter
来源：http://zaw.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://zgm.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uow.yj202588.top

JS:   get name() { return this._name; }
来源：http://qgh.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://byr.jiagoushi.top

Java: public String getName() { return name; }
来源：http://bdy.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vba.bjfxy.top

Ruby: attr_accessor :name
来源：http://gis.c1oappe.top

C#:   public string Name { get; set; }
来源：http://rag.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://tmy.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://ids.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wkl.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://lxf.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://zjt.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://wfe.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://lpq.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://oqt.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://sgu.yanxiufei.cn

[G13] 判断对象类型
来源：http://udh.yueranfly.top

Py:   isinstance(u, User)
来源：http://ael.hnqzz.top

PHP:  $u instanceof User
来源：http://pvj.dashuyun.cn

JS:   u instanceof User
来源：http://buc.jlsjyb.cn

TS:   u instanceof User
来源：http://fco.shangyingyoupin.top

Java: u instanceof User
来源：http://fmi.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pbx.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://bvn.tian-w.cn

C#:   u is User
来源：http://iar.zhiwuduotai.top

[G14] 数据类 / record
来源：http://jbw.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vxx.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://rxb.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vcx.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://cyl.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://mbn.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://xru.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqv.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://pem.ybcxt.top

[G15] 枚举
来源：http://mbf.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tkt.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://aty.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xvj.jinqigfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://isl.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://tps.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vky.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://cej.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cnb.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://etp.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://use.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://qeg.gogol.net.cn

JS:   Object.entries(obj)
来源：http://ali.ctjpmb.com

TS:   Object.entries(obj)
来源：http://lnu.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gsq.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ogm.yj202588.top

Ruby: obj.instance_variables
来源：http://pyp.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://muw.yfazqb.com

================================================================================
来源：http://bmy.smart0.xyz

H. 异常与错误处理
来源：http://dsa.zhiwuduotai.top

================================================================================
来源：http://tjm.xinyue.icu

[H01] try / catch 基础
来源：http://rnz.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pep.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://elg.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nmg.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vye.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xkz.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qaw.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tpq.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ugi.andypj.xyz

[H02] finally / ensure 收尾
来源：http://qoq.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mtf.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tuz.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bza.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ujc.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://zvz.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mfz.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xyd.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rne.zhengqikj.top

[H03] 主动抛出异常
来源：http://jfc.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://csr.fanxiaobao.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uqp.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://yxo.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://xga.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kxc.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://stz.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kid.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://xlu.smart0.xyz

[H04] 自定义异常类型
来源：http://fbi.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://lye.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://qtp.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://rfq.316326.xyz

TS:   class MyError extends Error {}
来源：http://afu.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://hsr.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vsr.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://zmj.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://rzv.ppjwa.cn

[H05] 捕获特定类型
来源：http://idj.yueranfly.top

Py:   except ValueError as e:
来源：http://yjy.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qsw.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://zkl.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://spr.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://twf.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ini.iojbl.cn

Ruby: rescue ArgumentError => e
来源：http://dkt.smart0.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tly.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://vff.cashguo.top

Py:   value = d.get("k") or default
来源：http://cou.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://thh.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://tun.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://kcn.xuetiantiany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://khc.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wrg.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://dwx.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://cqp.shanyushiyangtech.top

[H07] 断言
来源：http://ofo.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://ejx.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://tgq.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://kox.yj20258888.top

TS:   console.assert(x > 0);
来源：http://uwt.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://iqa.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kjh.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://irt.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://ttn.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://tzt.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://iyr.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fus.bbcook.cn

JS:   e.message;  e.stack
来源：http://dcs.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://evo.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mke.aizwys.cn

Go:   err.Error()
来源：http://gjb.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://hoo.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://jth.birdmap.top

[H09] 带错误码的异常
来源：http://lfr.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bwy.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://thl.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sre.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://awx.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ips.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://djc.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://khx.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rue.fktsv.cn

[H10] 资源自动释放
来源：http://oub.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zqx.epnwcf.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ixc.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vym.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dbz.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oip.snrcjt.cn

Go:   defer f.Close()
来源：http://jlx.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zya.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jqq.yfazqb.com

================================================================================
来源：http://pjl.cdnleiting.top

I. 正则表达式
来源：http://qvw.ctjpmb.com

================================================================================
来源：http://fgz.xylfe.cn

[I01] 判断是否匹配
来源：http://fdp.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jfa.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pus.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://pyh.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://acl.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mfv.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nbd.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://fob.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ozr.cdnleiting.top

[I02] 提取所有匹配
来源：http://rnt.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://iue.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rur.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ybv.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://roc.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fcp.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://akt.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://sxg.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fyq.aibaodan.cn

[I03] 提取捕获分组
来源：http://phc.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sdg.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qoe.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvt.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bra.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vhk.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jrn.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vdr.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hqt.hesvh.cn

[I04] 正则替换
来源：http://ubp.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aee.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fht.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://ibm.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://kcf.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nxp.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cqy.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oyj.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hoo.gaohongyu789.top

[I05] 按正则拆分
来源：http://tln.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zjv.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tfn.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://ino.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://ayw.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://big.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uql.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://lco.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hap.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qcx.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gsc.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eti.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://moo.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyh.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtp.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://scz.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jrz.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pib.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://acp.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yjh.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wbr.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://azy.snrcjt.cn

TS:   /error/gim
来源：http://gvx.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pck.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sec.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://jfi.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mxj.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://hde.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vfk.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsp.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kyh.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cza.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oxv.redwolf501.top


<!-- 参考信息 -->