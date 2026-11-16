代发 wailian999

[G02] 构造函数
来源：http://cfu.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://dlf.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://fbm.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://wpb.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://buh.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://qyz.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jkm.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://zev.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://feg.shuidangran.top

[G03] 实例属性
来源：http://mjo.gaohongyu789.top

Py:   self.name = "x"
来源：http://hyo.ctjpmb.com

PHP:  public string $name = "x";
来源：http://jfn.jyoumei.cn

JS:   this.name = "x";
来源：http://nsy.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://sai.feifeiyinyue.top

Java: private String name;
来源：http://jci.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://quj.zdqjudy.top

Ruby: @name = "x"
来源：http://fcu.ctjpmb.com

C#:   public string Name { get; set; } = "x";
来源：http://erh.hfpthk.cn

[G04] 定义方法
来源：http://nfo.zhengqikj.top

Py:   def greet(self): return self.name
来源：http://etx.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gil.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://uim.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://gqk.hywenlv.cn

Java: String greet() { return name; }
来源：http://pfl.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xrr.fengsongda.top

Ruby: def greet; @name; end
来源：http://rrq.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://iqu.birdmap.top

[G05] 继承
来源：http://suh.cucudq.cn

Py:   class Admin(User): pass
来源：http://thu.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://cki.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://lgv.hcnkem.com

TS:   class Admin extends User {}
来源：http://dyd.hysaishi.cn

Java: class Admin extends User {}
来源：http://cep.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wru.cqqwz.cn

Ruby: class Admin < User; end
来源：http://ndm.hnxiangtu.top

C#:   class Admin : User {}
来源：http://bzj.yj202588.top

[G06] 重写方法
来源：http://cza.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://sti.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dmr.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://lzv.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://hrn.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://ndu.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oid.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://kbn.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://xsp.hammf.cn

[G07] 调用父类方法
来源：http://yhi.bjfxy.top

Py:   super().greet()
来源：http://kqx.yuxming.cn

PHP:  parent::greet();
来源：http://zxm.hnqzz.top

JS:   super.greet();
来源：http://bov.hfpthk.cn

TS:   super.greet();
来源：http://xcx.xingfuxueyuan.xyz

Java: super.greet();
来源：http://wcu.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hcu.redwolf501.top

Ruby: super
来源：http://tnh.hnqzz.top

C#:   base.Greet();
来源：http://ljk.hammf.cn

[G08] 静态方法与属性
来源：http://ozy.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rtn.xinyue.icu

PHP:  public static function f() {}
来源：http://mbd.gotoacloud.top

JS:   static f() {}
来源：http://ocr.jinqigufen.top

TS:   static f(): void {}
来源：http://jtf.andypj.xyz

Java: static void f() {}
来源：http://bkg.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wji.mhx1999.top

Ruby: def self.f; end
来源：http://pla.9152youxi.cn

C#:   public static void F() {}
来源：http://xlm.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://dmy.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://odv.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://bhg.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ptv.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://pum.52xcode.cn

Java: interface Shape { double area(); }
来源：http://gvf.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://iav.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://foy.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://osy.316326.xyz

[G10] 访问控制
来源：http://dwy.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://tbc.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://jxn.havefunace.top

JS:   #private 字段；其余公开
来源：http://djj.haohaochexian.top

TS:   public / protected / private
来源：http://scq.cashguo.top

Java: public / protected / private / 默认包级
来源：http://zgj.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xsq.zhijiandao.cn

Ruby: public / protected / private
来源：http://uxs.yj20258888.top

C#:   public / protected / private / internal
来源：http://lou.bbcook.cn

[G11] getter / setter
来源：http://dyi.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://imn.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://yex.bjfxy.top

JS:   get name() { return this._name; }
来源：http://nsd.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://idm.fengsongda.top

Java: public String getName() { return name; }
来源：http://mpo.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rfb.jiagoushi.top

Ruby: attr_accessor :name
来源：http://skq.daria6918.cn

C#:   public string Name { get; set; }
来源：http://iqe.daxiang520.top

[G12] 对象转字符串
来源：http://det.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://xdw.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://spv.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://idk.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://lgw.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://fim.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gwm.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://kss.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://grm.bjfxy.top

[G13] 判断对象类型
来源：http://qhs.fktsv.cn

Py:   isinstance(u, User)
来源：http://akt.zycfv.cn

PHP:  $u instanceof User
来源：http://adr.gzhubu.top

JS:   u instanceof User
来源：http://jmh.zdbjq.cn

TS:   u instanceof User
来源：http://ljc.ydjk.org.cn

Java: u instanceof User
来源：http://ach.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dzd.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://kvz.dianchejie.cn

C#:   u is User
来源：http://pnk.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://jal.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tdc.tian-w.cn

PHP:  // 用 readonly 属性模拟
来源：http://put.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://fuf.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://yky.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://lru.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://dys.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ejl.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://koc.jqgufenzy.top

[G15] 枚举
来源：http://wjr.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vxq.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kkn.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ewm.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://med.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://zbn.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aju.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://fmq.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://scp.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://qhd.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nas.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://jvt.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://jrh.yfazqb.com

TS:   Object.entries(obj)
来源：http://gov.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://brg.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hjs.aizwys.cn

Ruby: obj.instance_variables
来源：http://gow.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://gmg.gzhubu.top

================================================================================
来源：http://rzq.jqgfzy.top

H. 异常与错误处理
来源：http://hum.shuidangran.top

================================================================================
来源：http://vpn.fktsv.cn

[H01] try / catch 基础
来源：http://rvo.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cst.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wji.fzhhl.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://esy.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xlz.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kjp.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xyc.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yue.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lnr.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://uvl.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://aci.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tzq.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ufq.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://toh.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mqv.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bxr.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ghn.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hwm.yueranfly.top

[H03] 主动抛出异常
来源：http://pcr.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://ykp.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ekh.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://clv.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://ckq.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tgo.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://grd.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lti.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://gwj.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://ymw.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://cky.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://zcu.ivvv.top

JS:   class MyError extends Error {}
来源：http://txx.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://hez.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://con.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zkb.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://cjz.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://vul.ctjpmb.com

[H05] 捕获特定类型
来源：http://tle.xuanzx.com

Py:   except ValueError as e:
来源：http://mif.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xue.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://bcy.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://xbm.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://mta.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yqk.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://tzh.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://san.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://bos.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://ttb.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://sul.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://ixf.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uuy.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wgi.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wbh.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://apw.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://xjl.xinyue.icu

[H07] 断言
来源：http://ccx.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://jqm.andypj.xyz

PHP:  assert($x > 0);
来源：http://jtk.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://nnu.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://ztx.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://zgp.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://orf.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ydy.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://jpu.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://puw.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://zgr.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cqy.yonumen.top

JS:   e.message;  e.stack
来源：http://jvs.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fqt.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hej.iojbl.cn

Go:   err.Error()
来源：http://jje.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://fxx.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://gvh.hfpthk.cn

[H09] 带错误码的异常
来源：http://skx.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kgp.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ezm.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cjq.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kcw.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://byt.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aov.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://dux.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hjv.yj202588.top

[H10] 资源自动释放
来源：http://oos.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://yov.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ezi.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ggu.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcn.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urz.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://yph.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ehg.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xbn.uphjek.com

================================================================================
来源：http://eky.jqgfzy.top

I. 正则表达式
来源：http://jca.shanyushiyangtech.top

================================================================================
来源：http://oww.xylfe.cn

[I01] 判断是否匹配
来源：http://ztj.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bxp.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://qoi.xylfe.cn

JS:   /\d+/.test(s)
来源：http://kwc.cucudq.cn

TS:   /\d+/.test(s)
来源：http://yjy.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://avz.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nep.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://mdp.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aks.snrcjt.cn

[I02] 提取所有匹配
来源：http://vry.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://hyc.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mcm.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xdj.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://gwe.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cjx.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qsz.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://osq.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fun.zhoulong.xyz

[I03] 提取捕获分组
来源：http://zmk.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ite.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pvh.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://edh.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pke.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jje.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://odl.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qoh.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mmt.shanyushiyangkeji.top

[I04] 正则替换
来源：http://wux.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uww.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rfc.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://jra.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mwv.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kjz.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://iic.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kqq.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ytw.aizwys.cn

[I05] 按正则拆分
来源：http://vrx.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ukc.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kdq.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://rkk.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://ewf.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://uyf.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mag.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://khc.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ldd.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pfw.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dhj.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://knz.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gel.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ule.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yrv.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ksi.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ezy.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vsf.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://dia.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://txz.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yms.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vzs.feifeiyinyue.top

TS:   /error/gim
来源：http://qcs.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yga.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jzc.yongpay.top

Ruby: s.scan(/error/i)
来源：http://ayi.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gol.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://dfm.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zih.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xjq.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlk.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyr.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://kzf.ydjk.org.cn


<!-- 参考信息 -->