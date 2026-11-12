代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://gbm.sufxvd.cn

[G03] 实例属性
来源：http://dbm.xuanzx.com

Py:   self.name = "x"
来源：http://pdb.nwbrower.top

PHP:  public string $name = "x";
来源：http://rzx.zhengqikj.top

JS:   this.name = "x";
来源：http://ewx.hesvh.cn

TS:   name: string = "x";
来源：http://fex.bjfxy.top

Java: private String name;
来源：http://fof.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nfe.gogol.net.cn

Ruby: @name = "x"
来源：http://jye.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://zec.zhiwuduotai.top

[G04] 定义方法
来源：http://zli.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://tsa.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gle.cheryme.top

JS:   greet() { return this.name; }
来源：http://ije.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://aga.xylfe.cn

Java: String greet() { return name; }
来源：http://knr.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jwv.guowangkeji.top

Ruby: def greet; @name; end
来源：http://ywo.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://bcu.jinghuilouyu.cn

[G05] 继承
来源：http://oar.tian-w.cn

Py:   class Admin(User): pass
来源：http://kky.pycfn.com

PHP:  class Admin extends User {}
来源：http://tfz.sufxvd.cn

JS:   class Admin extends User {}
来源：http://esl.cashguo.top

TS:   class Admin extends User {}
来源：http://jiv.jinqigufen.top

Java: class Admin extends User {}
来源：http://gpn.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hpd.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://iid.redwolf501.top

C#:   class Admin : User {}
来源：http://utt.yonumen.top

[G06] 重写方法
来源：http://sjr.tarul.cn

Py:   def greet(self): return "admin"
来源：http://zoo.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://igo.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://vzu.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://nea.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://cnw.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fer.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://ibf.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://qda.ivvv.top

[G07] 调用父类方法
来源：http://rxx.tian-w.cn

Py:   super().greet()
来源：http://qdl.tianlin.xyz

PHP:  parent::greet();
来源：http://eid.xinyue.icu

JS:   super.greet();
来源：http://grf.shzxlz.cn

TS:   super.greet();
来源：http://wui.jinqigfzy.top

Java: super.greet();
来源：http://yfp.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://smf.yangfankeji.com

Ruby: super
来源：http://ajp.xylfe.cn

C#:   base.Greet();
来源：http://hus.9152youxi.cn

[G08] 静态方法与属性
来源：http://pjf.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qcb.zhengqikj.top

PHP:  public static function f() {}
来源：http://jjc.cheryme.top

JS:   static f() {}
来源：http://plq.guannengcc.top

TS:   static f(): void {}
来源：http://lye.yangfankeji.com

Java: static void f() {}
来源：http://jqb.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pxx.dashuyun.cn

Ruby: def self.f; end
来源：http://amf.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://sry.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://vcu.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pgm.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bsh.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kav.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://zvi.52xcode.cn

Java: interface Shape { double area(); }
来源：http://jyl.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://hrg.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://azy.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://uio.jinqigufen.top

[G10] 访问控制
来源：http://ler.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://fbk.wangshuangyany.cn

PHP:  public / protected / private
来源：http://ydw.yueranfly.top

JS:   #private 字段；其余公开
来源：http://atd.uphjek.com

TS:   public / protected / private
来源：http://jzc.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://fvr.cqqwz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://poe.tianlin.xyz

Ruby: public / protected / private
来源：http://rmn.yvedp.cn

C#:   public / protected / private / internal
来源：http://sqa.smart0.xyz

[G11] getter / setter
来源：http://qtb.cashguo.top

Py:   @property 与 @x.setter
来源：http://zgi.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yty.yueranfly.top

JS:   get name() { return this._name; }
来源：http://lby.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://bov.aibaodan.cn

Java: public String getName() { return name; }
来源：http://wsa.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uic.jyoumei.cn

Ruby: attr_accessor :name
来源：http://idy.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://gdx.yvedp.cn

[G12] 对象转字符串
来源：http://dyd.jianghu66.top

Py:   def __str__(self): return self.name
来源：http://zaw.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oai.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://nfq.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://xlk.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://gwa.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://jbu.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://kul.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://koa.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://ooz.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://ogg.yuanzhike.top

PHP:  $u instanceof User
来源：http://fiy.shuidangran.top

JS:   u instanceof User
来源：http://tcg.chenlongwang.top

TS:   u instanceof User
来源：http://gxv.daxiang520.top

Java: u instanceof User
来源：http://fne.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bnb.yongpay.top

Ruby: u.is_a?(User)
来源：http://qii.daria6918.cn

C#:   u is User
来源：http://jeh.yongpay.top

[G14] 数据类 / record
来源：http://qfh.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vzr.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://kvh.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://yoe.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://nyq.fehbvm.com

Java: record User(String name, int age) {}
来源：http://uaa.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://fyf.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkw.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://qup.shangyingyoupin.top

[G15] 枚举
来源：http://moo.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://abx.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hht.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://quu.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dgh.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://ujg.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vdv.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://vbi.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqd.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ehn.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lzu.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://lmu.yonumen.top

JS:   Object.entries(obj)
来源：http://kqg.uphjek.com

TS:   Object.entries(obj)
来源：http://ksk.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdn.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wjc.yfazqb.com

Ruby: obj.instance_variables
来源：http://zcz.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://ojr.52xcode.cn

================================================================================
来源：http://qug.ivvv.top

H. 异常与错误处理
来源：http://nfx.hnxiangtu.top

================================================================================
来源：http://tkk.yonumen.top

[H01] try / catch 基础
来源：http://sww.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uzu.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mgi.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ofd.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aub.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gse.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://emv.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fga.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iba.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://fty.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://ihm.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ahc.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://anl.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bpu.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rok.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nvy.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://qei.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://fgt.hnxiangtu.top

[H03] 主动抛出异常
来源：http://gpm.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://lsw.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ljl.hammf.cn

JS:   throw new Error("错误信息");
来源：http://zte.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://zjc.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpm.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tgw.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rpw.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fyb.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://yim.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://fpp.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://gyu.xylfe.cn

JS:   class MyError extends Error {}
来源：http://mtk.sweek.top

TS:   class MyError extends Error {}
来源：http://elg.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://nen.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfy.tarul.cn

Ruby: class MyError < StandardError; end
来源：http://qzx.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://jsa.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://jsk.yanxiufei.cn

Py:   except ValueError as e:
来源：http://och.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rso.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://fny.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://yjd.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://udf.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mta.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://qcv.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://smj.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://kie.ybcxt.top

Py:   value = d.get("k") or default
来源：http://kjy.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://krw.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://xph.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://kbc.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zxk.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qtt.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://xzp.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://xxb.iojbl.cn

[H07] 断言
来源：http://kan.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://jxf.chenzaomai.com

PHP:  assert($x > 0);
来源：http://zvt.zycfv.cn

JS:   console.assert(x > 0);
来源：http://lbz.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://dht.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://qgp.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wqh.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://iwt.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://zbf.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://igl.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://jiu.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dnm.bjfxy.top

JS:   e.message;  e.stack
来源：http://uib.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gro.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://zsp.jinyuanbaomall.cn

Go:   err.Error()
来源：http://qts.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://ubd.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://ebv.nwbrower.top

[H09] 带错误码的异常
来源：http://cxk.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://emd.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aqe.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rjn.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sdc.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jfh.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sfz.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://xtn.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://twl.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://elz.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mot.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yxm.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pil.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bsm.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lzt.cheryme.top

Go:   defer f.Close()
来源：http://viz.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rnj.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ejj.9152youxi.cn

================================================================================
来源：http://scm.aibaodan.cn

I. 正则表达式
来源：http://wvi.shanyushiyangtech.top

================================================================================
来源：http://liz.andypj.xyz

[I01] 判断是否匹配
来源：http://iqi.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vle.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://zql.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://hsf.tanke756.top

TS:   /\d+/.test(s)
来源：http://rlb.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hcv.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jsd.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://bqz.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kkd.yongpay.top

[I02] 提取所有匹配
来源：http://jda.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://krx.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pyx.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://igh.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://vjq.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bfl.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gho.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://mbs.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eif.fehbvm.com

[I03] 提取捕获分组
来源：http://mix.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://leh.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xwl.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsc.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wgm.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xum.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://obw.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tzv.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bhx.xinyue.icu

[I04] 正则替换
来源：http://rlb.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rnw.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://umx.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://yrk.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://ese.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qfn.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ijp.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://phb.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eqw.cqqwz.cn

[I05] 按正则拆分
来源：http://xms.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iws.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sjs.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://jab.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://wtc.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://cgg.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tox.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zcy.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gbu.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mwi.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awi.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gwy.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mzz.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vrs.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ppi.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pjn.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cqr.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gxh.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://byx.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kta.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gpb.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vbo.shanyushiyangtech.top

TS:   /error/gim
来源：http://vbe.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lxe.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xae.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://bma.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ghp.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://sfl.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wyq.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bgh.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilb.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qss.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nkt.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ikc.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ohl.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ojb.yj20258888.top

================================================================================
来源：http://hjx.jinghuilouyu.cn

J. 日期与时间
来源：http://clh.zhengqikj.top

================================================================================
来源：http://yzv.sxryk.cn

[J01] 获取当前时间
来源：http://wzi.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://blw.sjlbkw.cn


<!-- 参考信息 -->