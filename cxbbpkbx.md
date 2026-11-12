代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://onm.bjfxy.top

JS:   greet() { return this.name; }
来源：http://dnc.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://itn.mhx1999.top

Java: String greet() { return name; }
来源：http://vmk.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aqo.yj20258.top

Ruby: def greet; @name; end
来源：http://wpk.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://rmq.ydjk.org.cn

[G05] 继承
来源：http://xow.cheryme.top

Py:   class Admin(User): pass
来源：http://mrh.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://ynr.chenlongwang.top

JS:   class Admin extends User {}
来源：http://vfm.jqgfzy.top

TS:   class Admin extends User {}
来源：http://ykl.316326.xyz

Java: class Admin extends User {}
来源：http://uwr.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uct.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://asb.jiagoushi.top

C#:   class Admin : User {}
来源：http://jkx.jinqigfzy.top

[G06] 重写方法
来源：http://hec.havefunace.top

Py:   def greet(self): return "admin"
来源：http://nnt.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://hwa.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://cqz.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://wxq.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://bmw.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqa.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://eax.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://nnv.tanke756.top

[G07] 调用父类方法
来源：http://goi.zdqjudy.top

Py:   super().greet()
来源：http://tme.ydzc1.top

PHP:  parent::greet();
来源：http://gwk.vehdjk.com

JS:   super.greet();
来源：http://fle.zhongyouzk.top

TS:   super.greet();
来源：http://ine.jinghuilouyu.cn

Java: super.greet();
来源：http://enp.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gbu.ydjk.org.cn

Ruby: super
来源：http://lzo.yj20258.top

C#:   base.Greet();
来源：http://rvh.snrcjt.cn

[G08] 静态方法与属性
来源：http://gon.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oxz.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://cef.sweek.top

JS:   static f() {}
来源：http://cpm.guowangkeji.top

TS:   static f(): void {}
来源：http://djc.xylfe.cn

Java: static void f() {}
来源：http://twc.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yvc.c1oappe.top

Ruby: def self.f; end
来源：http://oyz.wangdashe.top

C#:   public static void F() {}
来源：http://rdc.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://bnt.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://fvf.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://cda.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzi.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://opq.52xcode.cn

Java: interface Shape { double area(); }
来源：http://xyk.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://ahv.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dxu.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://hsf.guannengcc.top

[G10] 访问控制
来源：http://avz.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://syw.nanxuanxn.top

PHP:  public / protected / private
来源：http://moe.meibo888.top

JS:   #private 字段；其余公开
来源：http://nlw.yangfankeji.com

TS:   public / protected / private
来源：http://tvb.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://mnd.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://hyv.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://lgk.smart0.xyz

C#:   public / protected / private / internal
来源：http://aoi.meibo888.top

[G11] getter / setter
来源：http://jmz.wangdashe.top

Py:   @property 与 @x.setter
来源：http://vtw.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yio.ydzc1.top

JS:   get name() { return this._name; }
来源：http://mas.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://zbd.0kj1m.cn

Java: public String getName() { return name; }
来源：http://xpn.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://ozn.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://apj.cashguo.top

C#:   public string Name { get; set; }
来源：http://ksb.wangshuangyany.cn

[G12] 对象转字符串
来源：http://xvt.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://hnj.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nmw.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://stl.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://xhe.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://rqo.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://awx.andypj.xyz

Ruby: def to_s; @name; end
来源：http://zsw.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://yre.dashuyun.cn

[G13] 判断对象类型
来源：http://tfj.tanke756.top

Py:   isinstance(u, User)
来源：http://vtg.zhixingplan.top

PHP:  $u instanceof User
来源：http://uvl.yj20258888.top

JS:   u instanceof User
来源：http://wei.sjlbkw.cn

TS:   u instanceof User
来源：http://flt.jqgufenzy.top

Java: u instanceof User
来源：http://kyu.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvz.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://crx.feifeiyinyue.top

C#:   u is User
来源：http://tie.vehdjk.com

[G14] 数据类 / record
来源：http://gvi.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ypc.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://euj.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://pfm.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://nsd.shuidangran.top

Java: record User(String name, int age) {}
来源：http://lwq.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://xee.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xkz.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://efb.sjlbkw.cn

[G15] 枚举
来源：http://amj.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbe.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fis.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zgx.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xrh.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://anq.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jaq.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://jnx.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ipi.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://jqp.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nud.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://bva.sysykeji.top

JS:   Object.entries(obj)
来源：http://mjl.cdnleiting.top

TS:   Object.entries(obj)
来源：http://ait.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rmx.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ugt.yvedp.cn

Ruby: obj.instance_variables
来源：http://vsg.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://gmt.jinyuanbaomall.cn

================================================================================
来源：http://twx.hfpthk.cn

H. 异常与错误处理
来源：http://ksv.ppjwa.cn

================================================================================
来源：http://suq.uphjek.com

[H01] try / catch 基础
来源：http://aaf.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ewc.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fww.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://szf.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ywi.ctjpmb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ivz.yueranfly.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hsq.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dcq.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://shs.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://fvt.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://suf.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://axz.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uwb.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jvw.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://nvn.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bmi.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aqe.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wwq.jinqigufen.top

[H03] 主动抛出异常
来源：http://yje.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://zpw.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://llx.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://bki.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://wkj.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://smx.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sgw.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kjz.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://klh.jqgufenzy.top

[H04] 自定义异常类型
来源：http://pqi.jlsjyb.cn

Py:   class MyError(Exception): pass
来源：http://byl.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://qzi.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://ake.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://zua.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ifz.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xgi.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://ocn.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://cjt.sweek.top

[H05] 捕获特定类型
来源：http://eij.bjfxy.top

Py:   except ValueError as e:
来源：http://gzo.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wph.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://apt.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://jar.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://qyf.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://won.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://zvs.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sjy.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://cqx.tanke756.top

Py:   value = d.get("k") or default
来源：http://llj.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rsv.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lbz.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://doj.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sfp.zhijiandao.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hjn.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://luh.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://uex.svipenyu.cn

[H07] 断言
来源：http://ipy.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://zjy.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://dfo.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://mew.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://csm.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://doc.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dyp.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ukg.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://fmk.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://ack.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://btq.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bti.xziqi.cn

JS:   e.message;  e.stack
来源：http://fwy.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://fbf.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lhx.hnqzz.top

Go:   err.Error()
来源：http://clm.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://tme.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://lyl.ydzc1.top

[H09] 带错误码的异常
来源：http://wxy.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iga.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vbp.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://utm.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hib.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jpy.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vhp.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://yis.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://guu.cucudq.cn

[H10] 资源自动释放
来源：http://myf.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xxx.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rdo.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kcx.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vox.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xfb.aibaodan.cn

Go:   defer f.Close()
来源：http://euv.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vtk.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mae.52xcode.cn

================================================================================
来源：http://ccv.nanxinkj.top

I. 正则表达式
来源：http://krn.yj20258.top

================================================================================
来源：http://pyf.jyoumei.cn

[I01] 判断是否匹配
来源：http://qsn.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zvj.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://kbv.316326.xyz

JS:   /\d+/.test(s)
来源：http://rxd.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://zcw.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lul.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://omv.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://qsh.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cmy.jiagoushi.top

[I02] 提取所有匹配
来源：http://gyo.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://kmy.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ftg.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qzz.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://ctr.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nlu.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ekp.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://aqd.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nha.svipenyu.cn

[I03] 提取捕获分组
来源：http://xdk.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jmg.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yah.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bhj.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://onp.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kbb.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://owh.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uwa.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rwh.sweek.top

[I04] 正则替换
来源：http://juw.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nlp.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rue.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://tvk.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://yqn.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jkh.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ntv.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dfp.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://phn.hcnkem.com

[I05] 按正则拆分
来源：http://cqj.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zak.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mnn.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://biq.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://hdd.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://rms.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fwt.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://mug.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oyb.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bbc.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oju.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fbt.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kgf.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bbt.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://unh.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://scy.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cux.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cum.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://ynm.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gkm.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jen.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hss.mhx1999.top

TS:   /error/gim
来源：http://jlw.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fin.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tyq.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://epw.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rwc.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://fzl.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lej.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lzc.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fag.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yqr.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lrg.c1oappe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://syu.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eiq.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nlr.wangshuangyany.cn

================================================================================
来源：http://hqh.snrcjt.cn

J. 日期与时间
来源：http://fif.chenlongwang.top

================================================================================
来源：http://fem.haohaochexian.top

[J01] 获取当前时间
来源：http://dfq.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wip.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysr.xinyue.icu

JS:   new Date();  Date.now()
来源：http://zfz.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://xag.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://avr.fzhhl.top

Go:   time.Now()
来源：http://gjz.hammf.cn

Ruby: Time.now
来源：http://svr.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qhy.chenzaomai.com

[J02] 格式化输出
来源：http://ikk.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovn.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gat.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xxs.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://fku.ehwqpu.com


<!-- 参考信息 -->