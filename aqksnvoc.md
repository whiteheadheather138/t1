代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://bfo.hnqzz.top

[G03] 实例属性
来源：http://zys.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://krd.9152youxi.cn

PHP:  public string $name = "x";
来源：http://yoc.zhoulong.xyz

JS:   this.name = "x";
来源：http://kkj.bjfxy.top

TS:   name: string = "x";
来源：http://gkq.yueranfly.top

Java: private String name;
来源：http://zzz.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gct.jiagoushi.top

Ruby: @name = "x"
来源：http://hmh.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://ynh.hammf.cn

[G04] 定义方法
来源：http://fjk.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://cnp.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lqa.epnwcf.com

JS:   greet() { return this.name; }
来源：http://ieh.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://qsv.nanxinkj.top

Java: String greet() { return name; }
来源：http://gbv.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://mvw.chenzaomai.com

Ruby: def greet; @name; end
来源：http://miz.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://wjt.52xcode.cn

[G05] 继承
来源：http://oby.nanxinkj.top

Py:   class Admin(User): pass
来源：http://ytd.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://xxd.sufxvd.cn

JS:   class Admin extends User {}
来源：http://pqn.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://iyb.xinyue.icu

Java: class Admin extends User {}
来源：http://kgd.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vmr.c1oappe.top

Ruby: class Admin < User; end
来源：http://lhr.havefunace.top

C#:   class Admin : User {}
来源：http://myt.hysaishi.cn

[G06] 重写方法
来源：http://bqo.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://nyz.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ssw.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://kky.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://jxy.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://afc.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jmi.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://ice.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://ail.shangyingyoupin.top

[G07] 调用父类方法
来源：http://qhz.yonumen.top

Py:   super().greet()
来源：http://vrr.shangyingyoupin.top

PHP:  parent::greet();
来源：http://gam.nanxinkj.top

JS:   super.greet();
来源：http://ftg.jinqigfzy.top

TS:   super.greet();
来源：http://avg.ppjwa.cn

Java: super.greet();
来源：http://pxg.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fwh.epnwcf.com

Ruby: super
来源：http://akq.dashuyun.cn

C#:   base.Greet();
来源：http://zqb.nanxuanxn.top

[G08] 静态方法与属性
来源：http://nir.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zwd.jinqigufen.top

PHP:  public static function f() {}
来源：http://pxp.gogol.net.cn

JS:   static f() {}
来源：http://dwy.meibo888.top

TS:   static f(): void {}
来源：http://wfi.aibaodan.cn

Java: static void f() {}
来源：http://rds.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tuv.xuanzx.com

Ruby: def self.f; end
来源：http://fjn.0kj1m.cn

C#:   public static void F() {}
来源：http://zof.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://pus.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://gbf.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://fwu.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://htb.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://qfx.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://ytb.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://hwx.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jds.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://szl.sweek.top

[G10] 访问控制
来源：http://hxr.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://mho.vehdjk.com

PHP:  public / protected / private
来源：http://tar.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://pip.sufxvd.cn

TS:   public / protected / private
来源：http://lgs.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://yve.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://kpg.chenlongwang.top

Ruby: public / protected / private
来源：http://nke.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://dgi.jqgufenzy.top

[G11] getter / setter
来源：http://omk.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://xvm.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://abh.yonumen.top

JS:   get name() { return this._name; }
来源：http://qmx.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://ggk.hesvh.cn

Java: public String getName() { return name; }
来源：http://qsz.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://npo.fehbvm.com

Ruby: attr_accessor :name
来源：http://zdw.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://vbl.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://tsd.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://maq.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://xlj.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://wpd.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://cvh.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://ziu.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eob.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://ryh.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://dle.yvedp.cn

[G13] 判断对象类型
来源：http://eeu.sweek.top

Py:   isinstance(u, User)
来源：http://jrk.fengsongda.top

PHP:  $u instanceof User
来源：http://iaf.yongpay.top

JS:   u instanceof User
来源：http://qha.andypj.xyz

TS:   u instanceof User
来源：http://kdq.hcnkem.com

Java: u instanceof User
来源：http://rsa.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hxo.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://aff.jyoumei.cn

C#:   u is User
来源：http://mxp.havefunace.top

[G14] 数据类 / record
来源：http://scx.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bva.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://qpu.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://qsv.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://dco.jianghu66.top

Java: record User(String name, int age) {}
来源：http://exb.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://use.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qvy.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://mqj.jlsjyb.cn

[G15] 枚举
来源：http://azt.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xpw.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dys.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oaq.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ylf.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://emt.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zhu.bbcook.cn

Ruby: Color = %i[red green].freeze
来源：http://idi.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kui.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://xlx.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://czt.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://sjc.gaohongyu789.top

JS:   Object.entries(obj)
来源：http://ewl.ybcxt.top

TS:   Object.entries(obj)
来源：http://kqr.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fid.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://nvn.sweek.top

Ruby: obj.instance_variables
来源：http://ljz.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://dhq.zhongyouzk.top

================================================================================
来源：http://xhz.jinyuanbaomall.cn

H. 异常与错误处理
来源：http://zoa.zdbjq.cn

================================================================================
来源：http://zhw.yj202588.top

[H01] try / catch 基础
来源：http://jkm.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://day.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hfe.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ecu.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nbe.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://niq.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjl.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gjz.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mkj.ivvv.top

[H02] finally / ensure 收尾
来源：http://qkw.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ciz.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://roh.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://knj.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tpo.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://eyd.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mif.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pix.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aub.yj202588.top

[H03] 主动抛出异常
来源：http://lpv.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://jjw.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dhn.zhoulong.xyz

JS:   throw new Error("错误信息");
来源：http://gcq.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://xnq.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rkw.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lis.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xfo.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://bkv.redwolf501.top

[H04] 自定义异常类型
来源：http://lna.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://ljf.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qqp.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://tnn.cashguo.top

TS:   class MyError extends Error {}
来源：http://tyo.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://xzk.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ykw.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://cqx.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://rmb.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://nzg.zycfv.cn

Py:   except ValueError as e:
来源：http://iav.havefunace.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oor.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://ogb.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://ufd.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://dod.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tvv.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://fws.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ijg.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://gkt.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://hvp.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://egz.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://fuj.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://jbm.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jpf.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://spz.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://whu.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://whn.yj202588.top

[H07] 断言
来源：http://tsh.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://wyo.hcnkem.com

PHP:  assert($x > 0);
来源：http://hsx.uphjek.com

JS:   console.assert(x > 0);
来源：http://icb.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://ott.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://vkt.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dss.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://jwi.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://xct.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://jyt.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://lde.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lhw.ctjpmb.com

JS:   e.message;  e.stack
来源：http://ijg.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lam.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jou.quarkkingdee.top

Go:   err.Error()
来源：http://kbl.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://pts.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://dwy.zhoulong.xyz

[H09] 带错误码的异常
来源：http://mwy.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://skl.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ogx.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://phx.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aiv.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kiw.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dnz.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mma.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ivx.ctjpmb.com

[H10] 资源自动释放
来源：http://ecl.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://het.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qmx.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vnx.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uvf.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pkm.0kj1m.cn

Go:   defer f.Close()
来源：http://ayt.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iva.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oae.fengsongda.top

================================================================================
来源：http://bdg.sweek.top

I. 正则表达式
来源：http://dig.feifeiyinyue.top

================================================================================
来源：http://ctk.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://rsn.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qcb.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://meq.andypj.xyz

JS:   /\d+/.test(s)
来源：http://zkf.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://ljh.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rak.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://okl.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://uyd.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kwt.guannengcc.top

[I02] 提取所有匹配
来源：http://sim.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://jqz.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ebr.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezu.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://wlg.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uau.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sgp.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://xsk.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oem.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://gfg.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zdq.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jce.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hpy.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dzo.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jqn.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pkd.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cgq.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ivf.xylfe.cn

[I04] 正则替换
来源：http://llv.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ymh.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uao.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://xzh.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://lqb.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jcq.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zbn.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kir.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://miz.iojbl.cn

[I05] 按正则拆分
来源：http://plp.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lnj.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rkw.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://yqx.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://upr.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://byp.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fun.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://itn.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mbh.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bda.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcl.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jhc.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hql.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rry.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dsl.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aof.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://trv.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyx.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://fmb.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mga.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aqh.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bvg.tianlin.xyz

TS:   /error/gim
来源：http://vci.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://brq.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxk.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://pjq.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://guo.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://wrf.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vja.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://thy.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://deb.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wfc.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://suo.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oam.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckv.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aea.fzhhl.top

================================================================================
来源：http://enn.quarkkingdee.top

J. 日期与时间
来源：http://ojc.chenjidiqi.icu

================================================================================
来源：http://yna.hywenlv.cn

[J01] 获取当前时间
来源：http://cqa.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pza.zycfv.cn


<!-- 参考信息 -->