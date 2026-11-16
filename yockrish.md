代发 wailian999

TS:   constructor(public name: string) {}
来源：http://flq.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://mxy.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ffs.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://ehb.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://euv.jlsjyb.cn

[G03] 实例属性
来源：http://obx.snrcjt.cn

Py:   self.name = "x"
来源：http://ehp.xziqi.cn

PHP:  public string $name = "x";
来源：http://yyg.sysykeji.top

JS:   this.name = "x";
来源：http://qqk.tianlin.xyz

TS:   name: string = "x";
来源：http://wfa.shangyingyoupin.top

Java: private String name;
来源：http://pio.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://txw.jinqigfzy.top

Ruby: @name = "x"
来源：http://jnq.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://oma.shuidangran.top

[G04] 定义方法
来源：http://uiu.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://rhb.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://esz.cucudq.cn

JS:   greet() { return this.name; }
来源：http://xyk.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://ixr.cdnleiting.top

Java: String greet() { return name; }
来源：http://aip.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jci.zhixingplan.top

Ruby: def greet; @name; end
来源：http://mnl.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://mtn.gaohongyu789.top

[G05] 继承
来源：http://ibf.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://jym.ydzc1.top

PHP:  class Admin extends User {}
来源：http://ter.hesvh.cn

JS:   class Admin extends User {}
来源：http://uoi.birdmap.top

TS:   class Admin extends User {}
来源：http://ese.dashuyun.cn

Java: class Admin extends User {}
来源：http://ikl.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wdq.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://irh.kuanghao11.cn

C#:   class Admin : User {}
来源：http://msj.hongshengwenyu.top

[G06] 重写方法
来源：http://xsl.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://hwu.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zdr.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://pnj.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://mxw.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://qwm.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xay.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://oqr.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://uzh.yj202588.top

[G07] 调用父类方法
来源：http://nhr.jinghuilouyu.cn

Py:   super().greet()
来源：http://ubq.ppjwa.cn

PHP:  parent::greet();
来源：http://mjh.ywan-chungtsiang.top

JS:   super.greet();
来源：http://pmm.fehbvm.com

TS:   super.greet();
来源：http://wdi.hesvh.cn

Java: super.greet();
来源：http://tna.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yfz.redwolf501.top

Ruby: super
来源：http://ntc.9152youxi.cn

C#:   base.Greet();
来源：http://amn.zhengqikj.top

[G08] 静态方法与属性
来源：http://tud.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvn.tian-w.cn

PHP:  public static function f() {}
来源：http://zyo.chenlongwang.top

JS:   static f() {}
来源：http://fed.jiagoushi.top

TS:   static f(): void {}
来源：http://xaa.feifeiyinyue.top

Java: static void f() {}
来源：http://zxk.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hlc.hesvh.cn

Ruby: def self.f; end
来源：http://xru.9152youxi.cn

C#:   public static void F() {}
来源：http://xaq.smart0.xyz

[G09] 接口 / 抽象类
来源：http://efd.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://ifr.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://tay.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://brh.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://sfs.cashguo.top

Java: interface Shape { double area(); }
来源：http://jgb.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://ulh.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zww.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://gxa.yueranfly.top

[G10] 访问控制
来源：http://pcd.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://oat.0kj1m.cn

PHP:  public / protected / private
来源：http://tgl.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://vcf.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://eru.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://cdm.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tgq.wangshuangyany.cn

Ruby: public / protected / private
来源：http://xcn.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://tyr.jiagoushi.top

[G11] getter / setter
来源：http://vue.yuxming.cn

Py:   @property 与 @x.setter
来源：http://ind.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rxk.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://lfn.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://hpc.ppjwa.cn

Java: public String getName() { return name; }
来源：http://ees.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbf.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://mlv.daxiang520.top

C#:   public string Name { get; set; }
来源：http://pkg.fehbvm.com

[G12] 对象转字符串
来源：http://fmw.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://eqa.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://byi.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://ltv.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://ock.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://cla.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ezp.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://knu.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://gsr.cucudq.cn

[G13] 判断对象类型
来源：http://lhc.hammf.cn

Py:   isinstance(u, User)
来源：http://tkm.daria6918.cn

PHP:  $u instanceof User
来源：http://cds.smart0.xyz

JS:   u instanceof User
来源：http://hnn.yanxiufei.cn

TS:   u instanceof User
来源：http://lrm.hywenlv.cn

Java: u instanceof User
来源：http://gtt.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://eji.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://doh.hcnkem.com

C#:   u is User
来源：http://tut.yangfankeji.com

[G14] 数据类 / record
来源：http://jlq.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rrv.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://paz.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://xxq.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://vwo.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://sjy.yangfankeji.com

Go:   type User struct { Name string; Age int }
来源：http://jcj.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://trz.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://naa.havefunace.top

[G15] 枚举
来源：http://xjy.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://egh.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bfk.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dck.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://evb.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://aur.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rio.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://ich.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tug.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://emt.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ggc.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://boi.dianchejie.cn

JS:   Object.entries(obj)
来源：http://ewp.yonumen.top

TS:   Object.entries(obj)
来源：http://kvj.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dnq.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dpg.yueranfly.top

Ruby: obj.instance_variables
来源：http://avl.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://uft.yj20258.top

================================================================================
来源：http://msm.zycfv.cn

H. 异常与错误处理
来源：http://zsp.cucudq.cn

================================================================================
来源：http://nwl.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://umo.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pqj.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dia.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vtr.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zza.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rnp.ppjwa.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jnq.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nip.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ftw.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://ugd.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://lym.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://yxu.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lqm.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tyc.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://phb.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vlo.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://elo.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ota.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://ubb.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://voe.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ctb.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://szx.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://fxh.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://csj.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hyx.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rsm.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zhq.ivvv.top

[H04] 自定义异常类型
来源：http://vwr.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://aej.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://deg.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://cea.smart0.xyz

TS:   class MyError extends Error {}
来源：http://uiz.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://exn.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qfd.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://lzb.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://wrl.daxiang520.top

[H05] 捕获特定类型
来源：http://spu.9152youxi.cn

Py:   except ValueError as e:
来源：http://sao.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ykp.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://zpn.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://svm.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://wsf.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nhb.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://jwm.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://byo.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://mer.hnqzz.top

Py:   value = d.get("k") or default
来源：http://etx.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://wjd.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://bkb.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://lzl.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nkz.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hjw.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://kjk.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://vdc.bjfxy.top

[H07] 断言
来源：http://brv.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://bbk.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://ubt.cheryme.top

JS:   console.assert(x > 0);
来源：http://nim.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://ply.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://byi.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cdu.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bit.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://fqw.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://cbb.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://pry.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://umb.sweek.top

JS:   e.message;  e.stack
来源：http://xmi.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wxb.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ywj.birdmap.top

Go:   err.Error()
来源：http://rcb.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://tsu.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://pua.dashuyun.cn

[H09] 带错误码的异常
来源：http://lnd.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yhm.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xto.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://toy.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjb.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ckv.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rvi.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://gjo.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pcg.yueranfly.top

[H10] 资源自动释放
来源：http://ikz.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oud.ivvv.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://meo.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wws.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rkf.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ylr.daxiang520.top

Go:   defer f.Close()
来源：http://vem.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fuw.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://biy.xuetiantiany.cn

================================================================================
来源：http://emp.smart0.xyz

I. 正则表达式
来源：http://rsj.yj20258888.top

================================================================================
来源：http://xem.fzhhl.top

[I01] 判断是否匹配
来源：http://ack.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ora.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://tvo.yj202588.top

JS:   /\d+/.test(s)
来源：http://skn.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://tqq.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aml.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://auz.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://uxp.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vvi.ppjwa.cn

[I02] 提取所有匹配
来源：http://qkp.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://efj.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lvm.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://clo.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://gvk.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bxn.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uiu.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://efo.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gxx.hywenlv.cn

[I03] 提取捕获分组
来源：http://sty.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zqf.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tiv.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oca.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hov.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://acc.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rfh.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zyf.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://obs.epnwcf.com

[I04] 正则替换
来源：http://kwp.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://apu.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wnt.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://taw.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://bhv.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xgh.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dul.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zts.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fxt.hnqzz.top

[I05] 按正则拆分
来源：http://jvg.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ert.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ymq.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://nlv.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://jku.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://olj.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rze.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://duu.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://veo.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xvl.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nyv.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wcx.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vcz.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ojf.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ede.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpm.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qoz.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vrq.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://nif.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://taq.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bvd.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jsg.birdmap.top

TS:   /error/gim
来源：http://yqd.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ydm.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bew.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://sfy.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://emq.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://bew.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rao.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jrb.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://guw.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xka.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vah.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rwd.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jaa.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://duh.gaohongyu789.top

================================================================================
来源：http://rct.sysykeji.top


<!-- 参考信息 -->