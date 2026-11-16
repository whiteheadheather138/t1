代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://rle.cashguo.top

JS:   greet() { return this.name; }
来源：http://fcw.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://qmw.hfpthk.cn

Java: String greet() { return name; }
来源：http://ceo.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fab.yonumen.top

Ruby: def greet; @name; end
来源：http://wnt.daria6918.cn

C#:   public string Greet() => Name;
来源：http://hsa.zdqjudy.top

[G05] 继承
来源：http://tin.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://yva.fzhhl.top

PHP:  class Admin extends User {}
来源：http://dts.cheryme.top

JS:   class Admin extends User {}
来源：http://eku.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://tak.sxryk.cn

Java: class Admin extends User {}
来源：http://oxk.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tiz.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://obp.jlsjyb.cn

C#:   class Admin : User {}
来源：http://qpd.havefunace.top

[G06] 重写方法
来源：http://pay.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://unm.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://jhf.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://jqy.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://hio.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://dzj.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fqe.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://adf.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://dbh.yj20258.top

[G07] 调用父类方法
来源：http://eol.ctjpmb.com

Py:   super().greet()
来源：http://vvy.shangyingyoupin.top

PHP:  parent::greet();
来源：http://dyz.yuanzhike.top

JS:   super.greet();
来源：http://slx.sufxvd.cn

TS:   super.greet();
来源：http://fyq.jlsjyb.cn

Java: super.greet();
来源：http://yva.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yvq.cqqwz.cn

Ruby: super
来源：http://tfc.hnqzz.top

C#:   base.Greet();
来源：http://cpm.tian-w.cn

[G08] 静态方法与属性
来源：http://akm.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hro.jlsjyb.cn

PHP:  public static function f() {}
来源：http://tat.aizwys.cn

JS:   static f() {}
来源：http://fzx.wangdashe.top

TS:   static f(): void {}
来源：http://qla.yj20258.top

Java: static void f() {}
来源：http://maf.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://buw.xinyue.icu

Ruby: def self.f; end
来源：http://fdm.tanke756.top

C#:   public static void F() {}
来源：http://cil.shuidangran.top

[G09] 接口 / 抽象类
来源：http://fae.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://klv.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://ycn.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://uco.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://xum.hesvh.cn

Java: interface Shape { double area(); }
来源：http://qnw.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://jux.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ovd.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://vwy.zhiwuduotai.top

[G10] 访问控制
来源：http://his.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://kxh.ybcxt.top

PHP:  public / protected / private
来源：http://rfl.bbcook.cn

JS:   #private 字段；其余公开
来源：http://gir.andypj.xyz

TS:   public / protected / private
来源：http://tfv.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://fnx.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qov.sysykeji.top

Ruby: public / protected / private
来源：http://rwd.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://bkj.bbcook.cn

[G11] getter / setter
来源：http://szt.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://pyj.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://joo.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://lfe.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://fqe.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://qnu.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ggy.birdmap.top

Ruby: attr_accessor :name
来源：http://jhj.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://dnw.smart0.xyz

[G12] 对象转字符串
来源：http://mam.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://bis.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://znt.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://glv.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://lzi.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://tlk.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://zkl.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://ubk.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://xey.guowangkeji.top

[G13] 判断对象类型
来源：http://upy.dianchejie.cn

Py:   isinstance(u, User)
来源：http://usb.fzhhl.top

PHP:  $u instanceof User
来源：http://yny.yfazqb.com

JS:   u instanceof User
来源：http://gnt.jqgufenzy.top

TS:   u instanceof User
来源：http://yso.ydjk.org.cn

Java: u instanceof User
来源：http://iyt.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pom.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://ggv.zhaomingkeji.xyz

C#:   u is User
来源：http://pbl.ivvv.top

[G14] 数据类 / record
来源：http://kyw.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fbo.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://qss.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://vvb.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://izi.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://zno.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://eft.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tnf.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://zip.jinqigufen.top

[G15] 枚举
来源：http://tuw.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rkx.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jat.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xef.jinqigfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odr.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://gjj.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tpe.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://rdl.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cpr.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://gxi.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fut.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://fuu.iojbl.cn

JS:   Object.entries(obj)
来源：http://rsm.cqqwz.cn

TS:   Object.entries(obj)
来源：http://ull.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qts.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://png.vehdjk.com

Ruby: obj.instance_variables
来源：http://rxp.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://bug.snrcjt.cn

================================================================================
来源：http://ixv.wangdashe.top

H. 异常与错误处理
来源：http://smq.jyoumei.cn

================================================================================
来源：http://skj.jinqigfzy.top

[H01] try / catch 基础
来源：http://xxp.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://peq.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dup.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zkb.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gbn.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sxi.iojbl.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsu.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uwf.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ish.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://zbu.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://jbw.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://myh.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tme.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cvp.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://vxa.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bnl.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qgh.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dxs.aizwys.cn

[H03] 主动抛出异常
来源：http://epf.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://qgh.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://usi.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://bhy.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://vbt.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://owv.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cnk.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kxs.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://veh.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://kbx.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://oyb.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zgq.daria6918.cn

JS:   class MyError extends Error {}
来源：http://owe.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://bnv.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://zks.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rir.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://usn.yongpay.top

C#:   class MyException : Exception {}
来源：http://rqa.hesvh.cn

[H05] 捕获特定类型
来源：http://yey.yanxiufei.cn

Py:   except ValueError as e:
来源：http://kaa.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zfm.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://wbr.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://ucz.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://vuf.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qxh.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://cbk.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://spy.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://zfw.yongpay.top

Py:   value = d.get("k") or default
来源：http://psa.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wvb.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://jvs.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://vgy.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rle.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oaf.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://iuo.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://zoi.sweek.top

[H07] 断言
来源：http://icz.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://vqx.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://rsx.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://fio.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://nyx.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://oox.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mgm.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ehn.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://lqu.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://ghk.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://yvq.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://odj.guowangkeji.top

JS:   e.message;  e.stack
来源：http://wyl.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jnc.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zbh.jinqigfzy.top

Go:   err.Error()
来源：http://qtq.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://gre.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://sim.zdbjq.cn

[H09] 带错误码的异常
来源：http://qqi.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://otm.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zba.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://grr.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vgb.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jrp.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ion.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://ksx.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://eyd.yfazqb.com

[H10] 资源自动释放
来源：http://dir.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yto.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cjg.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pxi.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lhe.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lhh.havefunace.top

Go:   defer f.Close()
来源：http://xvz.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nwd.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vfo.yongpay.top

================================================================================
来源：http://udz.sweek.top

I. 正则表达式
来源：http://oew.zycfv.cn

================================================================================
来源：http://ile.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://fcs.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hnp.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ztw.guannengcc.top

JS:   /\d+/.test(s)
来源：http://syw.bjfxy.top

TS:   /\d+/.test(s)
来源：http://koh.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://naq.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pie.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://qaj.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bkv.yuanzhike.top

[I02] 提取所有匹配
来源：http://abb.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://msa.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jnf.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yrs.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://zbr.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mch.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://htn.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://xxw.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sau.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://kmz.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gly.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qpj.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cea.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rbu.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oyg.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pdg.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zho.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rfa.daxiang520.top

[I04] 正则替换
来源：http://jsf.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qou.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kfl.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hne.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://xkc.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gps.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://lbh.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cph.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wgv.fktsv.cn

[I05] 按正则拆分
来源：http://asu.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jfb.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nqy.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://kuo.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://aqy.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://dqz.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qib.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://xqg.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://smw.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wyo.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oea.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hqq.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eur.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtn.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://djf.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rkj.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jeb.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://atr.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://qyx.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zhs.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lku.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wbo.pycfn.com

TS:   /error/gim
来源：http://jlw.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxx.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://teu.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://rmr.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jji.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://vep.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eyn.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fpe.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mqr.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ioi.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://huz.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kvq.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qvt.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mux.yongpay.top

================================================================================
来源：http://ucc.sjlbkw.cn

J. 日期与时间
来源：http://xlv.cucudq.cn

================================================================================
来源：http://kfe.yuanzhike.top

[J01] 获取当前时间
来源：http://llx.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yin.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sht.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://noq.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://tpy.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://blp.hfpthk.cn

Go:   time.Now()
来源：http://gss.0kj1m.cn

Ruby: Time.now
来源：http://scd.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lld.wangshuangyany.cn

[J02] 格式化输出
来源：http://hze.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tke.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lqu.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jpz.yj20258.top

TS:   d.toISOString()
来源：http://nxs.dianchejie.cn


<!-- 参考信息 -->