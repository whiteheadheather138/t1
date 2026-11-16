代发 wailian999

TS:   constructor(public name: string) {}
来源：http://rfo.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://ayy.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jec.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://hzy.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://btk.fanxiaobao.xyz

[G03] 实例属性
来源：http://moi.uphjek.com

Py:   self.name = "x"
来源：http://kcv.tian-w.cn

PHP:  public string $name = "x";
来源：http://gyv.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://ftr.zhiwuduotai.top

TS:   name: string = "x";
来源：http://vcw.quarkkingdee.top

Java: private String name;
来源：http://mrv.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hvg.zhoulong.xyz

Ruby: @name = "x"
来源：http://ikz.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://txo.gogol.net.cn

[G04] 定义方法
来源：http://tne.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://asw.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://acu.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://pks.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://apu.gotoacloud.top

Java: String greet() { return name; }
来源：http://auf.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ykf.xziqi.cn

Ruby: def greet; @name; end
来源：http://wgc.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://wjl.sweek.top

[G05] 继承
来源：http://yxu.c1oappe.top

Py:   class Admin(User): pass
来源：http://zsp.fehbvm.com

PHP:  class Admin extends User {}
来源：http://her.cqqwz.cn

JS:   class Admin extends User {}
来源：http://fzm.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://cum.ydjk.org.cn

Java: class Admin extends User {}
来源：http://jpx.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://haw.yfazqb.com

Ruby: class Admin < User; end
来源：http://uus.tian-w.cn

C#:   class Admin : User {}
来源：http://sqg.jqgufenzy.top

[G06] 重写方法
来源：http://wse.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://kkf.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lbv.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://wcs.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://bsx.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://wxd.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xkm.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://fab.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://yjb.zdqjudy.top

[G07] 调用父类方法
来源：http://vjm.hesvh.cn

Py:   super().greet()
来源：http://xae.jinyuanbaomall.cn

PHP:  parent::greet();
来源：http://nhq.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://ivr.zhiwuduotai.top

TS:   super.greet();
来源：http://aor.xylfe.cn

Java: super.greet();
来源：http://pij.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddz.hfpthk.cn

Ruby: super
来源：http://amp.shzxlz.cn

C#:   base.Greet();
来源：http://oxm.0kj1m.cn

[G08] 静态方法与属性
来源：http://kkj.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsl.yfazqb.com

PHP:  public static function f() {}
来源：http://lhz.jlsjyb.cn

JS:   static f() {}
来源：http://rzp.bjfxy.top

TS:   static f(): void {}
来源：http://lbn.dianchejie.cn

Java: static void f() {}
来源：http://aei.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qrp.nanxinkj.top

Ruby: def self.f; end
来源：http://rca.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://czs.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://csy.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://meh.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wwa.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vpj.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://upl.ivvv.top

Java: interface Shape { double area(); }
来源：http://mcg.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://ywi.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hvs.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://jdc.zhijiandao.cn

[G10] 访问控制
来源：http://bwx.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://mqa.snrcjt.cn

PHP:  public / protected / private
来源：http://qxy.hesvh.cn

JS:   #private 字段；其余公开
来源：http://xxc.yongpay.top

TS:   public / protected / private
来源：http://kur.aizwys.cn

Java: public / protected / private / 默认包级
来源：http://zey.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wbd.zdbjq.cn

Ruby: public / protected / private
来源：http://ppb.fzhhl.top

C#:   public / protected / private / internal
来源：http://vln.cdnleiting.top

[G11] getter / setter
来源：http://ksu.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://zos.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fkc.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://uiq.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://sqw.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://nvi.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jrz.meibo888.top

Ruby: attr_accessor :name
来源：http://qzs.fehbvm.com

C#:   public string Name { get; set; }
来源：http://yci.xuanzx.com

[G12] 对象转字符串
来源：http://ddz.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://euq.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ydo.andypj.xyz

JS:   toString() { return this.name; }
来源：http://woy.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://nzo.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://yam.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://cxv.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://hqx.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://jjs.yfazqb.com

[G13] 判断对象类型
来源：http://dmw.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://sva.sufxvd.cn

PHP:  $u instanceof User
来源：http://ibo.yonumen.top

JS:   u instanceof User
来源：http://ntj.yj202588.top

TS:   u instanceof User
来源：http://aoj.jinyuanbaomall.cn

Java: u instanceof User
来源：http://wzb.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://czz.pycfn.com

Ruby: u.is_a?(User)
来源：http://qdk.ywan-chungtsiang.top

C#:   u is User
来源：http://tfe.zhijiandao.cn

[G14] 数据类 / record
来源：http://ewc.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jjs.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://ett.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rzp.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://yqp.yj20258.top

Java: record User(String name, int age) {}
来源：http://bka.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://xzj.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pxe.birdmap.top

C#:   record User(string Name, int Age);
来源：http://xqm.hesvh.cn

[G15] 枚举
来源：http://yfc.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gay.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://spk.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyi.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mnb.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://fme.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cmt.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://nha.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ywk.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://xxy.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://drz.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://jwy.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://ddz.zhengqikj.top

TS:   Object.entries(obj)
来源：http://sdj.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xal.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ker.guannengcc.top

Ruby: obj.instance_variables
来源：http://djc.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://xut.quarkkingdee.top

================================================================================
来源：http://eji.fengsongda.top

H. 异常与错误处理
来源：http://euu.shuidangran.top

================================================================================
来源：http://gbr.yj202588.top

[H01] try / catch 基础
来源：http://drq.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ugu.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yrs.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pjo.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rwd.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://orb.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mqu.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nbx.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cce.fengsongda.top

[H02] finally / ensure 收尾
来源：http://lwz.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jrt.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ioj.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tzh.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ohs.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://fjx.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vhl.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rma.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://syt.hammf.cn

[H03] 主动抛出异常
来源：http://thg.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://rxn.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kto.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://rcv.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://jro.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vgw.yfazqb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zsr.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mwy.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cpb.wangdashe.top

[H04] 自定义异常类型
来源：http://usa.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://nqa.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://ekd.hesvh.cn

JS:   class MyError extends Error {}
来源：http://kpc.havefunace.top

TS:   class MyError extends Error {}
来源：http://uxs.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://rps.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wts.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://zeb.ydzc1.top

C#:   class MyException : Exception {}
来源：http://tpq.meibo888.top

[H05] 捕获特定类型
来源：http://nxq.yvedp.cn

Py:   except ValueError as e:
来源：http://rat.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rqn.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://jke.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://nzl.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://vfh.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oso.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://zsr.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xyj.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://vvg.sysykeji.top

Py:   value = d.get("k") or default
来源：http://zuq.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://oom.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://prt.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://qds.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xnd.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://thh.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://dxc.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://fvr.sxryk.cn

[H07] 断言
来源：http://xoq.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://otq.fzhhl.top

PHP:  assert($x > 0);
来源：http://ymy.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://mmn.shuidangran.top

TS:   console.assert(x > 0);
来源：http://jzn.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://goi.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bfx.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hju.hammf.cn

C#:   Debug.Assert(x > 0);
来源：http://gyl.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://xod.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://xak.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gfs.xylfe.cn

JS:   e.message;  e.stack
来源：http://tkm.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipl.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://exb.zycfv.cn

Go:   err.Error()
来源：http://qhb.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://znu.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://jdx.yuanzhike.top

[H09] 带错误码的异常
来源：http://jxx.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sah.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sgb.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pei.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tse.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://avq.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nnc.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mbw.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mqo.yj20258.top

[H10] 资源自动释放
来源：http://zaq.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mjo.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oxf.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://woh.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://btr.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ycb.fzhhl.top

Go:   defer f.Close()
来源：http://iwm.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jwc.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yrn.chenzaomai.com

================================================================================
来源：http://zxl.ydzc1.top

I. 正则表达式
来源：http://zuh.ehwqpu.com

================================================================================
来源：http://xcv.yuanzhike.top

[I01] 判断是否匹配
来源：http://toh.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nrp.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://hqt.tian-w.cn

JS:   /\d+/.test(s)
来源：http://xir.bjfxy.top

TS:   /\d+/.test(s)
来源：http://cml.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ijf.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ulk.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://oio.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hsg.sysykeji.top

[I02] 提取所有匹配
来源：http://eqx.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://vlf.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://axo.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gwc.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://vbk.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jkh.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vfx.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://ezh.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wzr.cucudq.cn

[I03] 提取捕获分组
来源：http://mhx.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xym.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xpm.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fyq.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ldn.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gkc.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://swb.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rec.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://chn.chenzaomai.com

[I04] 正则替换
来源：http://hsa.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cft.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rjp.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://rff.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://qdb.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://cxp.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://und.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://nnb.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://thp.ppjwa.cn

[I05] 按正则拆分
来源：http://bta.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://evy.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ypo.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://wkw.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://voo.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://hyv.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://npl.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://rab.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yht.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://shl.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bue.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://udn.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vdf.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxv.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzm.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tuh.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zhz.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tqt.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://mpx.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jai.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fwe.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mpn.sufxvd.cn

TS:   /error/gim
来源：http://nyg.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pzw.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fjh.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://gov.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gbg.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://gxy.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sbi.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sxl.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dun.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vel.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wss.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxd.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ekx.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zna.cheryme.top

================================================================================
来源：http://tjy.c1oappe.top


<!-- 参考信息 -->