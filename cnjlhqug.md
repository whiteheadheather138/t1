代发 wailian999

JS:   this.name = "x";
来源：http://wiq.nwbrower.top

TS:   name: string = "x";
来源：http://rdc.wangshuangyany.cn

Java: private String name;
来源：http://hzl.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dtv.guannengcc.top

Ruby: @name = "x"
来源：http://seh.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://ygb.svipenyu.cn

[G04] 定义方法
来源：http://stj.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://myy.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dbk.jianghu66.top

JS:   greet() { return this.name; }
来源：http://avd.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://jou.xinyue.icu

Java: String greet() { return name; }
来源：http://vqk.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdy.bjfxy.top

Ruby: def greet; @name; end
来源：http://jfk.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://fzf.ctjpmb.com

[G05] 继承
来源：http://uky.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://okc.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://cfv.0kj1m.cn

JS:   class Admin extends User {}
来源：http://qlt.sysykeji.top

TS:   class Admin extends User {}
来源：http://iim.havefunace.top

Java: class Admin extends User {}
来源：http://dam.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zrw.haohaochexian.top

Ruby: class Admin < User; end
来源：http://iob.xziqi.cn

C#:   class Admin : User {}
来源：http://frf.c1oappe.top

[G06] 重写方法
来源：http://cnl.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://xvo.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://epj.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://ycb.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://fhh.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://phr.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://buy.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://pij.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://dfc.dashuyun.cn

[G07] 调用父类方法
来源：http://qop.fanxiaobao.xyz

Py:   super().greet()
来源：http://ige.uphjek.com

PHP:  parent::greet();
来源：http://lks.hcnkem.com

JS:   super.greet();
来源：http://taz.wangdashe.top

TS:   super.greet();
来源：http://sta.fktsv.cn

Java: super.greet();
来源：http://qtp.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gqp.jinqigfzy.top

Ruby: super
来源：http://ptw.yfazqb.com

C#:   base.Greet();
来源：http://lyx.cheryme.top

[G08] 静态方法与属性
来源：http://tce.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zkv.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://krt.chenlongwang.top

JS:   static f() {}
来源：http://mza.9152youxi.cn

TS:   static f(): void {}
来源：http://fnr.cashguo.top

Java: static void f() {}
来源：http://yyn.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cxk.cqqwz.cn

Ruby: def self.f; end
来源：http://gkp.fzhhl.top

C#:   public static void F() {}
来源：http://ahk.hammf.cn

[G09] 接口 / 抽象类
来源：http://lfv.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://fep.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://uxs.fzhhl.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ncm.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://rno.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://ije.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://irw.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lar.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://wyq.pengpengdd.cyou

[G10] 访问控制
来源：http://thp.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://wnx.jlsjyb.cn

PHP:  public / protected / private
来源：http://sqq.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://qfm.yj20258888.top

TS:   public / protected / private
来源：http://qoc.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://yyc.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fdn.9152youxi.cn

Ruby: public / protected / private
来源：http://hot.yfazqb.com

C#:   public / protected / private / internal
来源：http://rpz.fehbvm.com

[G11] getter / setter
来源：http://cxx.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://gbo.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wvt.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://ryn.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://uxq.yuanzhike.top

Java: public String getName() { return name; }
来源：http://baq.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rea.cqqwz.cn

Ruby: attr_accessor :name
来源：http://cql.xinyue.icu

C#:   public string Name { get; set; }
来源：http://elu.shangyingyoupin.top

[G12] 对象转字符串
来源：http://nry.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://cvd.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://get.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://fvv.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://mlo.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://zcv.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qtc.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://ivd.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://vgo.yueranfly.top

[G13] 判断对象类型
来源：http://nms.yj20258888.top

Py:   isinstance(u, User)
来源：http://prq.tarul.cn

PHP:  $u instanceof User
来源：http://cju.0kj1m.cn

JS:   u instanceof User
来源：http://qmc.jyoumei.cn

TS:   u instanceof User
来源：http://jhv.jqgfzy.top

Java: u instanceof User
来源：http://qtt.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gpl.xziqi.cn

Ruby: u.is_a?(User)
来源：http://jtr.dashuyun.cn

C#:   u is User
来源：http://vdy.ybcxt.top

[G14] 数据类 / record
来源：http://tgb.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aom.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://hqq.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qpo.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://zgr.yj20258.top

Java: record User(String name, int age) {}
来源：http://qsv.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://lly.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://set.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ivd.ehwqpu.com

[G15] 枚举
来源：http://zal.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xsb.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lyc.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cym.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ese.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://bmm.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ice.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://ocr.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mfa.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://bga.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://csd.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://net.yueranfly.top

JS:   Object.entries(obj)
来源：http://equ.yj202588.top

TS:   Object.entries(obj)
来源：http://tfi.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://clr.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbv.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://pun.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://fgn.yvedp.cn

================================================================================
来源：http://iwt.jqgfzy.top

H. 异常与错误处理
来源：http://yzw.9152youxi.cn

================================================================================
来源：http://eek.fktsv.cn

[H01] try / catch 基础
来源：http://rgg.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ljn.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://atq.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ssx.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wep.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fii.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jcq.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://znp.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gwt.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://zbs.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ryg.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qpj.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vfj.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://rhp.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://kuu.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pym.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ocb.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ozc.ehwqpu.com

[H03] 主动抛出异常
来源：http://vwd.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://kor.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cul.yj202588.top

JS:   throw new Error("错误信息");
来源：http://bxh.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://dme.nanxinkj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kyw.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjm.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lmd.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zpn.jyoumei.cn

[H04] 自定义异常类型
来源：http://dyu.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://aqc.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yql.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://mft.jianghu66.top

TS:   class MyError extends Error {}
来源：http://ioy.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://bcl.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vuz.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://lmc.fengsongda.top

C#:   class MyException : Exception {}
来源：http://gqs.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://klw.52xcode.cn

Py:   except ValueError as e:
来源：http://keg.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fdx.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://anz.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://vvs.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://qku.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jiv.yonumen.top

Ruby: rescue ArgumentError => e
来源：http://pmu.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pne.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://pin.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://pju.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://thb.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://akf.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://hdc.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tlr.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ezl.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://rhu.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://lkk.redwolf501.top

[H07] 断言
来源：http://tvv.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://viz.jianghu66.top

PHP:  assert($x > 0);
来源：http://rsp.bbcook.cn

JS:   console.assert(x > 0);
来源：http://lic.jiagoushi.top

TS:   console.assert(x > 0);
来源：http://hcb.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://rgm.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pdy.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://ifb.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://zjn.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://aer.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://xjw.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ejv.dianchejie.cn

JS:   e.message;  e.stack
来源：http://stt.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://myv.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://num.shuidangran.top

Go:   err.Error()
来源：http://bsf.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://tpu.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://bey.jqgufenzy.top

[H09] 带错误码的异常
来源：http://xrn.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://szj.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://aia.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://brk.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rmi.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fnj.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://siw.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://uvn.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://frc.zhixingplan.top

[H10] 资源自动释放
来源：http://huq.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sfe.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uvv.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dxo.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pgu.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://idd.aizwys.cn

Go:   defer f.Close()
来源：http://rre.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fax.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ahw.zdbjq.cn

================================================================================
来源：http://vfv.nanxuanxn.top

I. 正则表达式
来源：http://ojv.haohaochexian.top

================================================================================
来源：http://rsb.fehbvm.com

[I01] 判断是否匹配
来源：http://cap.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wme.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://aau.meibo888.top

JS:   /\d+/.test(s)
来源：http://srd.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://gwi.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wuf.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://til.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://azt.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivy.chenzaomai.com

[I02] 提取所有匹配
来源：http://bwa.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://jnc.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ofy.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wdw.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://kgu.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sbx.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://joo.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://cpu.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://phh.ydzc1.top

[I03] 提取捕获分组
来源：http://hci.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lky.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gis.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rtb.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oyj.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://csp.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ryx.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dpj.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vmf.havefunace.top

[I04] 正则替换
来源：http://pni.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vgj.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://har.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://plr.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://mqg.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://pbt.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://qlm.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://vvi.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zqq.iojbl.cn

[I05] 按正则拆分
来源：http://pan.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bzj.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cri.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://wvm.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://fen.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://kfi.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nhq.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mgh.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ooh.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ezo.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vqu.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qua.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qyp.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dwo.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ckx.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nyi.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uwj.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kpx.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://plx.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tpy.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zsc.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://svi.zdbjq.cn

TS:   /error/gim
来源：http://onx.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://elh.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ild.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://iks.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yfp.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://uhc.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://njj.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbb.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ubl.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pvh.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ilj.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dge.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ial.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lfe.cheryme.top

================================================================================
来源：http://eyx.sufxvd.cn

J. 日期与时间
来源：http://aus.yueranfly.top

================================================================================
来源：http://gzx.xuanzx.com

[J01] 获取当前时间
来源：http://kkr.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bon.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zvs.xinyue.icu

JS:   new Date();  Date.now()
来源：http://ebo.zycfv.cn

TS:   new Date();  Date.now()
来源：http://tsd.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://amn.daria6918.cn


<!-- 参考信息 -->