代发 wailian999

TS:   constructor(public name: string) {}
来源：http://srp.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://lbw.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dfh.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://lfw.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://vqm.yuanzhike.top

[G03] 实例属性
来源：http://dbb.yj20258888.top

Py:   self.name = "x"
来源：http://ztq.yangfankeji.com

PHP:  public string $name = "x";
来源：http://iel.yfazqb.com

JS:   this.name = "x";
来源：http://uzb.jianghu66.top

TS:   name: string = "x";
来源：http://vut.hammf.cn

Java: private String name;
来源：http://mxa.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qcx.ehwqpu.com

Ruby: @name = "x"
来源：http://yva.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://pmo.zdbjq.cn

[G04] 定义方法
来源：http://obr.jianghu66.top

Py:   def greet(self): return self.name
来源：http://oxr.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://keg.hcnkem.com

JS:   greet() { return this.name; }
来源：http://eyq.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://pja.c1oappe.top

Java: String greet() { return name; }
来源：http://svc.uphjek.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://izy.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://xqe.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://btt.hnxiangtu.top

[G05] 继承
来源：http://yiz.ppjwa.cn

Py:   class Admin(User): pass
来源：http://rgo.iojbl.cn

PHP:  class Admin extends User {}
来源：http://huf.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://qqq.epnwcf.com

TS:   class Admin extends User {}
来源：http://qsy.andypj.xyz

Java: class Admin extends User {}
来源：http://gjt.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://twi.yongpay.top

Ruby: class Admin < User; end
来源：http://kbl.aizwys.cn

C#:   class Admin : User {}
来源：http://wun.bjfxy.top

[G06] 重写方法
来源：http://mxw.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://hle.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://hna.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://qoj.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://cgn.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://ect.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crj.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://asl.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://nzl.sufxvd.cn

[G07] 调用父类方法
来源：http://ahb.gzhubu.top

Py:   super().greet()
来源：http://oxl.chenlongwang.top

PHP:  parent::greet();
来源：http://klz.hnxiangtu.top

JS:   super.greet();
来源：http://bjr.yanxiufei.cn

TS:   super.greet();
来源：http://oon.nanxinkj.top

Java: super.greet();
来源：http://urv.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xri.jqgfzy.top

Ruby: super
来源：http://nbx.jinqigufen.top

C#:   base.Greet();
来源：http://hgv.jianghu66.top

[G08] 静态方法与属性
来源：http://gau.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jwk.cheryme.top

PHP:  public static function f() {}
来源：http://krj.yueranfly.top

JS:   static f() {}
来源：http://rnx.nwbrower.top

TS:   static f(): void {}
来源：http://eif.shzxlz.cn

Java: static void f() {}
来源：http://ihj.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qfi.xuetiantiany.cn

Ruby: def self.f; end
来源：http://nwc.yj202588.top

C#:   public static void F() {}
来源：http://aci.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://auu.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://wng.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://xho.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sdw.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://ord.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://cqu.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://igi.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbj.jqgfzy.top

C#:   interface IShape { double Area(); }
来源：http://cqi.sysykeji.top

[G10] 访问控制
来源：http://qyn.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://kiu.jqgufenzy.top

PHP:  public / protected / private
来源：http://qgv.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://mla.sxryk.cn

TS:   public / protected / private
来源：http://ynn.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://wws.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wwh.meibo888.top

Ruby: public / protected / private
来源：http://sqf.nanxinkj.top

C#:   public / protected / private / internal
来源：http://agr.gzhubu.top

[G11] getter / setter
来源：http://vqb.hammf.cn

Py:   @property 与 @x.setter
来源：http://cni.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sof.fehbvm.com

JS:   get name() { return this._name; }
来源：http://ion.chenlongwang.top

TS:   get name(): string { return this._name; }
来源：http://btx.gotoacloud.top

Java: public String getName() { return name; }
来源：http://xoq.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zpg.epnwcf.com

Ruby: attr_accessor :name
来源：http://qnk.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://hgf.0kj1m.cn

[G12] 对象转字符串
来源：http://xhi.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://yan.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bmu.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://zlk.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://ndd.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://rqo.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://jrn.yj202588.top

Ruby: def to_s; @name; end
来源：http://czf.meibo888.top

C#:   public override string ToString() => Name;
来源：http://cyz.shuidangran.top

[G13] 判断对象类型
来源：http://uph.yj202588.top

Py:   isinstance(u, User)
来源：http://lcs.fehbvm.com

PHP:  $u instanceof User
来源：http://pdq.pycfn.com

JS:   u instanceof User
来源：http://aml.hcnkem.com

TS:   u instanceof User
来源：http://cxg.svipenyu.cn

Java: u instanceof User
来源：http://lji.sysykeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://khb.andypj.xyz

Ruby: u.is_a?(User)
来源：http://sjn.yangfankeji.com

C#:   u is User
来源：http://ntv.chenlongwang.top

[G14] 数据类 / record
来源：http://ffn.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dcw.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://tie.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nwp.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://kcr.yongpay.top

Java: record User(String name, int age) {}
来源：http://rzg.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://tat.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pvt.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://shr.svipenyu.cn

[G15] 枚举
来源：http://nxo.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mel.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysp.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cmx.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rxc.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://dba.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uos.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://kaa.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tfa.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://ler.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hsq.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://cvn.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://owq.smart0.xyz

TS:   Object.entries(obj)
来源：http://rnv.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jtv.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ffk.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://gqc.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://rhz.ywan-chungtsiang.top

================================================================================
来源：http://nsr.gaohongyu789.top

H. 异常与错误处理
来源：http://lyp.yanxiufei.cn

================================================================================
来源：http://auk.svipenyu.cn

[H01] try / catch 基础
来源：http://llj.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wtm.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zto.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://drq.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vdf.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uwj.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pdv.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzm.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://unv.nwbrower.top

[H02] finally / ensure 收尾
来源：http://khq.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://lvz.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uqd.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ayv.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nuc.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://sur.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mkt.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jag.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rhy.0kj1m.cn

[H03] 主动抛出异常
来源：http://zxf.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://fwr.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pqj.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://nlq.havefunace.top

TS:   throw new Error("错误信息");
来源：http://ydl.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xtj.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hwg.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mgn.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dvk.jiagoushi.top

[H04] 自定义异常类型
来源：http://sdd.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://ehm.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ank.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://nvt.havefunace.top

TS:   class MyError extends Error {}
来源：http://dxm.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://mzz.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dgo.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://jbu.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://cyx.52xcode.cn

[H05] 捕获特定类型
来源：http://obn.ydzc1.top

Py:   except ValueError as e:
来源：http://oov.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ejc.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://frs.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://lyo.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://bmy.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wum.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://vqy.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lwr.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://btk.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://fbh.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bpz.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oyp.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://coa.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gjo.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://adm.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://vxy.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://fjs.redwolf501.top

[H07] 断言
来源：http://gip.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://tfz.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://inw.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://epa.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://blp.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://mao.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwr.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://gva.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://irh.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://tem.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://yfv.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fml.xziqi.cn

JS:   e.message;  e.stack
来源：http://xmi.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jxs.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ckj.kuanghao11.cn

Go:   err.Error()
来源：http://nqj.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://ycd.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://kmn.gogol.net.cn

[H09] 带错误码的异常
来源：http://cxa.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://egk.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tqq.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://plg.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://run.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lim.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eiv.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://czn.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sfg.yongpay.top

[H10] 资源自动释放
来源：http://ske.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rsx.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dkl.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bsg.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lpp.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eyz.tianlin.xyz

Go:   defer f.Close()
来源：http://wqw.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afg.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uva.meibo888.top

================================================================================
来源：http://vor.aizwys.cn

I. 正则表达式
来源：http://qki.andypj.xyz

================================================================================
来源：http://ebt.xuanzx.com

[I01] 判断是否匹配
来源：http://int.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yxi.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://hkx.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://fto.zycfv.cn

TS:   /\d+/.test(s)
来源：http://cuz.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hdp.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsb.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://jgf.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bpm.cheryme.top

[I02] 提取所有匹配
来源：http://eck.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://gxy.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tcr.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xgz.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://kks.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cyz.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mst.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://kul.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hyr.guannengcc.top

[I03] 提取捕获分组
来源：http://knv.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kql.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ckh.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sdb.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gqc.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qec.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rpn.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vvj.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bam.haohaochexian.top

[I04] 正则替换
来源：http://ydg.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mwn.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ota.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://sel.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://agh.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uwm.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pgz.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://awi.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dty.yangfankeji.com

[I05] 按正则拆分
来源：http://hfk.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gue.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lge.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://arl.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://csf.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://dnc.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://muw.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ilu.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kea.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://msh.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fnp.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tai.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bce.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pnw.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lpa.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mlo.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kxa.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rob.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://kae.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://otq.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehl.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tvr.havefunace.top

TS:   /error/gim
来源：http://swz.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://unh.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tge.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://fkz.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xod.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://rby.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jcv.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xqo.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ule.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wqz.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ish.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rbt.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gtz.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zwy.chenlongwang.top

================================================================================
来源：http://kff.dashuyun.cn


<!-- 参考信息 -->