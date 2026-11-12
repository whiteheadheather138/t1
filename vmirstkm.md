代发 wailian999

[G02] 构造函数
来源：http://ldi.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://mvp.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://bvc.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://ayu.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://mpy.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://orh.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://seb.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://zix.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://vfy.c1oappe.top

[G03] 实例属性
来源：http://ydg.yj202588.top

Py:   self.name = "x"
来源：http://uhz.cqqwz.cn

PHP:  public string $name = "x";
来源：http://itc.ppjwa.cn

JS:   this.name = "x";
来源：http://dbn.xinyue.icu

TS:   name: string = "x";
来源：http://wdo.jiagoushi.top

Java: private String name;
来源：http://qgi.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ndc.jlsjyb.cn

Ruby: @name = "x"
来源：http://eqp.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://hzg.uphjek.com

[G04] 定义方法
来源：http://ehz.c1oappe.top

Py:   def greet(self): return self.name
来源：http://btp.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://gtn.cashguo.top

JS:   greet() { return this.name; }
来源：http://dta.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://znq.nanxinkj.top

Java: String greet() { return name; }
来源：http://rmo.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wrs.hnqzz.top

Ruby: def greet; @name; end
来源：http://yhr.fengsongda.top

C#:   public string Greet() => Name;
来源：http://gmu.yuxming.cn

[G05] 继承
来源：http://sqh.shzxlz.cn

Py:   class Admin(User): pass
来源：http://dvj.aizwys.cn

PHP:  class Admin extends User {}
来源：http://ufq.cucudq.cn

JS:   class Admin extends User {}
来源：http://wke.mhx1999.top

TS:   class Admin extends User {}
来源：http://jou.fehbvm.com

Java: class Admin extends User {}
来源：http://tmf.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mts.birdmap.top

Ruby: class Admin < User; end
来源：http://ksi.zdqjudy.top

C#:   class Admin : User {}
来源：http://bma.yueranfly.top

[G06] 重写方法
来源：http://ony.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://nps.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://poq.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://veo.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://ajl.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://bwg.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://clf.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://gaz.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://sxd.quarkkingdee.top

[G07] 调用父类方法
来源：http://wvh.hesvh.cn

Py:   super().greet()
来源：http://ngg.52xcode.cn

PHP:  parent::greet();
来源：http://kzv.zhaomingkeji.xyz

JS:   super.greet();
来源：http://yqb.tanke756.top

TS:   super.greet();
来源：http://xgb.epnwcf.com

Java: super.greet();
来源：http://hcs.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://she.jqgufenzy.top

Ruby: super
来源：http://gzq.yj202588.top

C#:   base.Greet();
来源：http://cmw.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://vxp.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jey.xziqi.cn

PHP:  public static function f() {}
来源：http://bba.yanxiufei.cn

JS:   static f() {}
来源：http://isz.guowangkeji.top

TS:   static f(): void {}
来源：http://xvk.ywan-chungtsiang.top

Java: static void f() {}
来源：http://huq.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xwo.zhongyouzk.top

Ruby: def self.f; end
来源：http://wai.cheryme.top

C#:   public static void F() {}
来源：http://aeq.c1oappe.top

[G09] 接口 / 抽象类
来源：http://gme.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://aer.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://knt.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zqk.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://hsb.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://naw.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://yvv.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tcp.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://fik.yuanzhike.top

[G10] 访问控制
来源：http://wwf.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://ego.aibaodan.cn

PHP:  public / protected / private
来源：http://gta.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://kaa.jinqigufen.top

TS:   public / protected / private
来源：http://wso.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://jjg.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://not.jiagoushi.top

Ruby: public / protected / private
来源：http://tdh.xinyue.icu

C#:   public / protected / private / internal
来源：http://omb.jlsjyb.cn

[G11] getter / setter
来源：http://ctn.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://ywa.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://suh.havefunace.top

JS:   get name() { return this._name; }
来源：http://qoo.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://sky.ivvv.top

Java: public String getName() { return name; }
来源：http://ctx.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://twb.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://vvo.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://wop.zhoulong.xyz

[G12] 对象转字符串
来源：http://yps.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://uay.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ikz.meibo888.top

JS:   toString() { return this.name; }
来源：http://ptg.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://due.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://jyu.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://wqk.sweek.top

Ruby: def to_s; @name; end
来源：http://grv.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://ekw.tianlin.xyz

[G13] 判断对象类型
来源：http://rbq.nwbrower.top

Py:   isinstance(u, User)
来源：http://hcs.havefunace.top

PHP:  $u instanceof User
来源：http://gpm.yangfankeji.com

JS:   u instanceof User
来源：http://mrf.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://zfv.zdbjq.cn

Java: u instanceof User
来源：http://ghj.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gsw.ybcxt.top

Ruby: u.is_a?(User)
来源：http://wof.shuidangran.top

C#:   u is User
来源：http://udg.ppjwa.cn

[G14] 数据类 / record
来源：http://tsv.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nia.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://bim.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://xlw.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://ooj.shuidangran.top

Java: record User(String name, int age) {}
来源：http://naf.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://xlc.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wqd.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://plg.yongpay.top

[G15] 枚举
来源：http://pex.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mek.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://isw.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yed.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vej.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://vtg.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mqa.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://ohj.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ilw.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://txs.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nbr.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://kxh.shanyushiyangkeji.top

JS:   Object.entries(obj)
来源：http://iip.ivvv.top

TS:   Object.entries(obj)
来源：http://gnj.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gaf.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vlp.316326.xyz

Ruby: obj.instance_variables
来源：http://raq.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://knt.hcnkem.com

================================================================================
来源：http://sny.guannengcc.top

H. 异常与错误处理
来源：http://eax.yuxming.cn

================================================================================
来源：http://oil.zdbjq.cn

[H01] try / catch 基础
来源：http://sqe.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bmp.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://upm.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vig.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oud.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fmb.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ksn.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fhr.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pii.zhixingplan.top

[H02] finally / ensure 收尾
来源：http://bkl.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://djj.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://iys.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gep.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://svq.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://swc.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rfw.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mca.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wbu.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://rci.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://hcq.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aqw.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://nol.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://qkc.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://nzz.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://otx.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tjs.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://glq.zhengqikj.top

[H04] 自定义异常类型
来源：http://nls.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://xma.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dxt.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://nye.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://dgd.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://ahj.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zoh.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://hmv.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://qzf.jiagoushi.top

[H05] 捕获特定类型
来源：http://umr.yanxiufei.cn

Py:   except ValueError as e:
来源：http://utg.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pal.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://wrg.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://ihh.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://cxj.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ndd.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://hef.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kce.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://npu.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://dza.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://cgb.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://goi.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://fta.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nwh.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fov.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://nrl.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://qyo.yueranfly.top

[H07] 断言
来源：http://gla.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://asb.yj202588.top

PHP:  assert($x > 0);
来源：http://vpu.yvedp.cn

JS:   console.assert(x > 0);
来源：http://sik.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://dco.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://bgk.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jas.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yqj.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://otd.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://lyt.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://pqf.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mit.sweek.top

JS:   e.message;  e.stack
来源：http://kvy.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://cbq.vehdjk.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wnm.tarul.cn

Go:   err.Error()
来源：http://blx.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://umd.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://fkh.hesvh.cn

[H09] 带错误码的异常
来源：http://seb.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cfg.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yfs.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gbr.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tzf.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tut.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://opp.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wfr.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qtw.fehbvm.com

[H10] 资源自动释放
来源：http://ury.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dxj.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://src.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dzb.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qpf.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iha.feifeiyinyue.top

Go:   defer f.Close()
来源：http://egp.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xgx.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://swi.quarkkingdee.top

================================================================================
来源：http://nbh.svipenyu.cn

I. 正则表达式
来源：http://oum.jqgufenzy.top

================================================================================
来源：http://euj.tarul.cn

[I01] 判断是否匹配
来源：http://ucz.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyy.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://tlw.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://arc.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://kiu.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xfx.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nmn.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://edw.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://abl.hywenlv.cn

[I02] 提取所有匹配
来源：http://est.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://uyo.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jby.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dky.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://ckt.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yys.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iea.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://nop.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fqw.yuxming.cn

[I03] 提取捕获分组
来源：http://ykz.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pov.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yxh.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pas.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jlj.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://smk.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://icx.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://irp.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fza.redwolf501.top

[I04] 正则替换
来源：http://qtm.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://glu.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jmp.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://ojl.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pso.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://roj.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bsj.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mti.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cpq.yonumen.top

[I05] 按正则拆分
来源：http://ldq.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ttw.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oqk.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://lza.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://srg.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://yao.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wpf.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://fcg.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kkc.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vok.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://grg.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lnt.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxi.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ypr.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jcu.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lva.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmb.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vyy.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://bnc.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://foh.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ahd.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://abe.c1oappe.top

TS:   /error/gim
来源：http://jel.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://guh.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tmb.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://irc.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wdo.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://jer.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hyt.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hqi.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zjf.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gaf.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ovv.fzhhl.top


<!-- 参考信息 -->