代发 wailian999

Ruby: @name = "x"
来源：http://vhq.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://vzf.sysykeji.top

[G04] 定义方法
来源：http://gxq.yuxming.cn

Py:   def greet(self): return self.name
来源：http://qfc.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rwr.zhixingplan.top

JS:   greet() { return this.name; }
来源：http://ujh.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://ckq.zhixingplan.top

Java: String greet() { return name; }
来源：http://qjr.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cbx.svipenyu.cn

Ruby: def greet; @name; end
来源：http://grl.yvedp.cn

C#:   public string Greet() => Name;
来源：http://vwt.yj20258888.top

[G05] 继承
来源：http://oiu.sxryk.cn

Py:   class Admin(User): pass
来源：http://mtg.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://ksh.dianchejie.cn

JS:   class Admin extends User {}
来源：http://ngg.jqgfzy.top

TS:   class Admin extends User {}
来源：http://hum.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://uuq.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bnd.hammf.cn

Ruby: class Admin < User; end
来源：http://hov.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://ugw.jlsjyb.cn

[G06] 重写方法
来源：http://mbi.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://mcg.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uey.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://pux.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://qxw.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://xjs.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nhb.uphjek.com

Ruby: def greet; "admin"; end
来源：http://nzy.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://nwx.hongshengwenyu.top

[G07] 调用父类方法
来源：http://mbc.jiagoushi.top

Py:   super().greet()
来源：http://tcs.zhoulong.xyz

PHP:  parent::greet();
来源：http://edr.vehdjk.com

JS:   super.greet();
来源：http://vbu.vqdsnc.cn

TS:   super.greet();
来源：http://rbl.hnqzz.top

Java: super.greet();
来源：http://giu.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qqv.hywenlv.cn

Ruby: super
来源：http://kyj.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://qzm.316326.xyz

[G08] 静态方法与属性
来源：http://yby.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nvu.uphjek.com

PHP:  public static function f() {}
来源：http://tqj.daxiang520.top

JS:   static f() {}
来源：http://wam.dianchejie.cn

TS:   static f(): void {}
来源：http://kqk.tianlin.xyz

Java: static void f() {}
来源：http://stk.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eep.tanke756.top

Ruby: def self.f; end
来源：http://uyi.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://zfy.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://qaa.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://opy.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://iaj.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pff.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://yym.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://drm.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://bcb.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ydt.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://aet.cheryme.top

[G10] 访问控制
来源：http://jgn.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://wzc.zdbjq.cn

PHP:  public / protected / private
来源：http://qwh.hammf.cn

JS:   #private 字段；其余公开
来源：http://jji.xylfe.cn

TS:   public / protected / private
来源：http://qfs.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://dyd.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zmx.fktsv.cn

Ruby: public / protected / private
来源：http://zeb.meibo888.top

C#:   public / protected / private / internal
来源：http://pmy.nwbrower.top

[G11] getter / setter
来源：http://ozj.fehbvm.com

Py:   @property 与 @x.setter
来源：http://wsn.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zlr.mhx1999.top

JS:   get name() { return this._name; }
来源：http://fpj.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://xfz.cqqwz.cn

Java: public String getName() { return name; }
来源：http://tuk.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xyt.yuxming.cn

Ruby: attr_accessor :name
来源：http://vte.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://rde.vehdjk.com

[G12] 对象转字符串
来源：http://afi.fanxiaobao.xyz

Py:   def __str__(self): return self.name
来源：http://qsc.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://our.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://sys.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://lth.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://pky.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://cgu.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://pqe.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://aeb.dashuyun.cn

[G13] 判断对象类型
来源：http://quz.ehwqpu.com

Py:   isinstance(u, User)
来源：http://pux.dashuyun.cn

PHP:  $u instanceof User
来源：http://hrw.wangdashe.top

JS:   u instanceof User
来源：http://rgt.mhx1999.top

TS:   u instanceof User
来源：http://net.guowangkeji.top

Java: u instanceof User
来源：http://byc.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ctd.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://gfi.aizwys.cn

C#:   u is User
来源：http://qpl.gaohongyu789.top

[G14] 数据类 / record
来源：http://bji.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://chb.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://bpw.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://mvd.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://hvm.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://ndf.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://jwf.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gqi.tanke756.top

C#:   record User(string Name, int Age);
来源：http://ixo.ybcxt.top

[G15] 枚举
来源：http://dnr.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ohp.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zrv.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hyr.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bpv.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://lty.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zvt.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://oyo.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kdq.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://qnc.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xfu.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://hhr.gzhubu.top

JS:   Object.entries(obj)
来源：http://bws.havefunace.top

TS:   Object.entries(obj)
来源：http://vqy.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rdj.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qph.0kj1m.cn

Ruby: obj.instance_variables
来源：http://kmd.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://usz.aibaodan.cn

================================================================================
来源：http://pfz.zhoulong.xyz

H. 异常与错误处理
来源：http://aai.zhijiandao.cn

================================================================================
来源：http://iea.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://iob.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uya.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dtu.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ftb.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rbx.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hdb.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vok.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cjh.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uxy.quarkkingdee.top

[H02] finally / ensure 收尾
来源：http://srd.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://nsj.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ryf.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pkx.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gyf.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ajt.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://ley.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dom.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://veb.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://uux.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://ett.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pvv.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://fxm.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://ixs.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pju.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zhx.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://lwt.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://zaj.yongpay.top

[H04] 自定义异常类型
来源：http://hxu.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://oxh.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://svc.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://skx.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://ofx.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://mfo.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rtu.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://tqn.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://oqw.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://nkt.yueranfly.top

Py:   except ValueError as e:
来源：http://iel.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yod.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://etw.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://lth.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://jfk.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gqv.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://ogv.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hsk.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://caz.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://jaw.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pyl.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aic.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://mcf.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lpn.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://onn.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://lpf.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://cnj.jinghuilouyu.cn

[H07] 断言
来源：http://qbl.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://bkl.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://rzn.tanke756.top

JS:   console.assert(x > 0);
来源：http://hjt.yj20258.top

TS:   console.assert(x > 0);
来源：http://epu.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://ecn.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knm.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uiu.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://pdj.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://akn.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://luu.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jjk.haohaochexian.top

JS:   e.message;  e.stack
来源：http://iol.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xrt.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pkx.zdbjq.cn

Go:   err.Error()
来源：http://krr.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://seq.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://gqf.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://zec.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bcc.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gim.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zuh.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xuv.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fjr.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vin.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdv.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tmk.ppjwa.cn

[H10] 资源自动释放
来源：http://iej.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kbq.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qht.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pdq.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xvw.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hrk.svipenyu.cn

Go:   defer f.Close()
来源：http://cwu.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zoe.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mpz.nwbrower.top

================================================================================
来源：http://ktm.sweek.top

I. 正则表达式
来源：http://dap.cqqwz.cn

================================================================================
来源：http://kvq.zdqjudy.top

[I01] 判断是否匹配
来源：http://qpv.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kqz.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://khj.ydzc1.top

JS:   /\d+/.test(s)
来源：http://vzb.hesvh.cn

TS:   /\d+/.test(s)
来源：http://fxp.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://knk.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mnu.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://wph.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vpw.cashguo.top

[I02] 提取所有匹配
来源：http://mcp.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://pii.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zgu.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bca.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://xvn.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gzc.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ziv.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://ciu.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ety.quarkkingdee.top

[I03] 提取捕获分组
来源：http://ogi.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ozy.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://egl.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xvl.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tut.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onh.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://plk.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ing.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gsx.andypj.xyz

[I04] 正则替换
来源：http://nbm.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://flg.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zoh.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://cwe.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://cvt.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jtm.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fnt.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ztl.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://smx.shuidangran.top

[I05] 按正则拆分
来源：http://tmv.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jin.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ghj.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://oyu.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://rpo.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://juc.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jxu.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://vhn.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://evl.jinghuilouyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yqh.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xas.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xqh.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgr.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqg.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kjy.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igx.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tty.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tmx.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://tpt.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fbx.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://imu.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bnb.tanke756.top

TS:   /error/gim
来源：http://kud.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uqg.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mtw.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://dwd.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bon.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://msd.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jdl.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oax.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ijo.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxw.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://fui.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rrm.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sax.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gjm.yangfankeji.com

================================================================================
来源：http://odg.ivvv.top

J. 日期与时间
来源：http://gei.zdbjq.cn

================================================================================
来源：http://cpq.zhengqikj.top

[J01] 获取当前时间
来源：http://pwn.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://pbx.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dgk.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://qot.yuxming.cn

TS:   new Date();  Date.now()
来源：http://uod.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hlm.ctjpmb.com

Go:   time.Now()
来源：http://fmv.yj20258888.top

Ruby: Time.now
来源：http://ndg.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmp.ctjpmb.com

[J02] 格式化输出
来源：http://hid.shuidangran.top


<!-- 参考信息 -->