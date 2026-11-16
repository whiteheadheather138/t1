代发 wailian999

Ruby: @name = "x"
来源：http://ikg.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://yoh.bjfxy.top

[G04] 定义方法
来源：http://xki.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://bll.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://edh.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://oru.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://urf.uphjek.com

Java: String greet() { return name; }
来源：http://axq.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nwr.cqqwz.cn

Ruby: def greet; @name; end
来源：http://rkg.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://uui.jianghu66.top

[G05] 继承
来源：http://arm.zdqjudy.top

Py:   class Admin(User): pass
来源：http://vrp.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://wkz.yangfankeji.com

JS:   class Admin extends User {}
来源：http://jwa.uphjek.com

TS:   class Admin extends User {}
来源：http://pra.yangfankeji.com

Java: class Admin extends User {}
来源：http://njz.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://abt.hcnkem.com

Ruby: class Admin < User; end
来源：http://veu.cdnleiting.top

C#:   class Admin : User {}
来源：http://jqq.zhongyouzk.top

[G06] 重写方法
来源：http://lfh.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://lvn.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jhl.cheryme.top

JS:   greet() { return "admin"; }
来源：http://unl.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://dvw.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ebr.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lnt.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://udw.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://fpk.tanke756.top

[G07] 调用父类方法
来源：http://zlu.jinyuanbaomall.cn

Py:   super().greet()
来源：http://tfu.yvedp.cn

PHP:  parent::greet();
来源：http://nvp.meibo888.top

JS:   super.greet();
来源：http://him.zhijiandao.cn

TS:   super.greet();
来源：http://pwx.sjlbkw.cn

Java: super.greet();
来源：http://klu.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yrw.gotoacloud.top

Ruby: super
来源：http://ehy.gogol.net.cn

C#:   base.Greet();
来源：http://qft.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://zmr.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ysv.haohaochexian.top

PHP:  public static function f() {}
来源：http://wln.vehdjk.com

JS:   static f() {}
来源：http://jdi.gzhubu.top

TS:   static f(): void {}
来源：http://tjl.shuidangran.top

Java: static void f() {}
来源：http://zpy.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dfe.vehdjk.com

Ruby: def self.f; end
来源：http://qop.xinyue.icu

C#:   public static void F() {}
来源：http://pkz.fktsv.cn

[G09] 接口 / 抽象类
来源：http://kxj.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://mdm.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xca.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ubv.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://ipn.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://ttw.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://rtv.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xqr.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://ldk.chenzaomai.com

[G10] 访问控制
来源：http://wkb.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://vgn.yuanzhike.top

PHP:  public / protected / private
来源：http://ban.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://dgw.hysaishi.cn

TS:   public / protected / private
来源：http://ggk.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://oyy.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrc.haohaochexian.top

Ruby: public / protected / private
来源：http://lei.hammf.cn

C#:   public / protected / private / internal
来源：http://jna.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://ekh.fktsv.cn

Py:   @property 与 @x.setter
来源：http://rvd.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dfr.zycfv.cn

JS:   get name() { return this._name; }
来源：http://nyn.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://ljv.hysaishi.cn

Java: public String getName() { return name; }
来源：http://ibq.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wyv.tarul.cn

Ruby: attr_accessor :name
来源：http://iup.smart0.xyz

C#:   public string Name { get; set; }
来源：http://hcm.bbcook.cn

[G12] 对象转字符串
来源：http://vgw.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://zhd.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zso.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://jxl.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://yhb.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://ppb.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://swf.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://ild.jinqigufen.top

C#:   public override string ToString() => Name;
来源：http://cel.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://gld.hammf.cn

Py:   isinstance(u, User)
来源：http://xnv.nanxuanxn.top

PHP:  $u instanceof User
来源：http://juc.uphjek.com

JS:   u instanceof User
来源：http://kss.jinqigufen.top

TS:   u instanceof User
来源：http://ket.bbcook.cn

Java: u instanceof User
来源：http://dhl.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bvq.ivvv.top

Ruby: u.is_a?(User)
来源：http://coj.sxryk.cn

C#:   u is User
来源：http://zmd.hfpthk.cn

[G14] 数据类 / record
来源：http://qsj.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yzw.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://raa.nanxuanxn.top

JS:   // 无内置：普通类或对象字面量
来源：http://lbj.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://dtf.redwolf501.top

Java: record User(String name, int age) {}
来源：http://mih.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://max.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iat.hammf.cn

C#:   record User(string Name, int Age);
来源：http://dqf.chenlongwang.top

[G15] 枚举
来源：http://mjv.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pih.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://pbn.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pdx.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gzk.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://ozz.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tow.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://rsz.gotoacloud.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zqt.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://lll.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cyw.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://odz.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://wak.sweek.top

TS:   Object.entries(obj)
来源：http://uno.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://drl.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fws.yj202588.top

Ruby: obj.instance_variables
来源：http://kuu.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://ktf.dianchejie.cn

================================================================================
来源：http://zkp.9152youxi.cn

H. 异常与错误处理
来源：http://san.guowangkeji.top

================================================================================
来源：http://spo.ydjk.org.cn

[H01] try / catch 基础
来源：http://sqd.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://chj.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ldz.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ohg.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yvu.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://arn.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xmg.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jeb.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://int.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://sob.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://pvx.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dgv.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zbv.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lts.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://ewe.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hrg.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ibn.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://mkk.ybcxt.top

[H03] 主动抛出异常
来源：http://vlp.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://tdh.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wih.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://sgc.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://ltz.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wmh.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://evn.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ubs.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://txd.xziqi.cn

[H04] 自定义异常类型
来源：http://nai.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://hjg.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://edf.yongpay.top

JS:   class MyError extends Error {}
来源：http://bvg.yongpay.top

TS:   class MyError extends Error {}
来源：http://tmm.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://gwi.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jjg.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://grp.xinyue.icu

C#:   class MyException : Exception {}
来源：http://fjf.jqgfzy.top

[H05] 捕获特定类型
来源：http://jtz.yj202588.top

Py:   except ValueError as e:
来源：http://yzx.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://khh.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://wgo.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://svo.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://iad.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oul.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://ahh.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jpp.xingfuxueyuan.xyz

[H06] 可选值 / 空值安全访问
来源：http://tzt.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://wzk.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ldq.zhixingplan.top

JS:   obj?.a?.b;  d ?? default
来源：http://vra.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://jof.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yia.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lty.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://mcy.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://lan.xingfuxueyuan.xyz

[H07] 断言
来源：http://xmp.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://ykd.jyoumei.cn

PHP:  assert($x > 0);
来源：http://wpv.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://syr.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://gow.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://pth.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndy.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://njp.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://ucc.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://jyq.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://vhc.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cha.fktsv.cn

JS:   e.message;  e.stack
来源：http://yfb.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://onm.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tzm.xuetiantiany.cn

Go:   err.Error()
来源：http://umk.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://hoj.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://rsa.cdnleiting.top

[H09] 带错误码的异常
来源：http://jhj.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fhp.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fpg.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vke.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cjq.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tmv.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gsg.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cpq.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qka.feifeiyinyue.top

[H10] 资源自动释放
来源：http://wys.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oqg.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jac.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xdp.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mxf.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lqy.ctjpmb.com

Go:   defer f.Close()
来源：http://sfu.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mco.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yeb.zhixingplan.top

================================================================================
来源：http://zre.yangfankeji.com

I. 正则表达式
来源：http://rpl.bjfxy.top

================================================================================
来源：http://idd.ivvv.top

[I01] 判断是否匹配
来源：http://wps.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://unb.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gut.tanke756.top

JS:   /\d+/.test(s)
来源：http://dfw.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://cfe.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ovc.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eiw.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://aat.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znv.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://ecs.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://zdm.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fuy.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tpa.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://vsk.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wpa.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zks.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://jdq.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ixa.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://nlm.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ioj.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dfl.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ruc.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fsm.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eps.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bcz.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pax.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://djw.chenzaomai.com

[I04] 正则替换
来源：http://rui.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zlt.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gbl.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pwb.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://aeu.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ofs.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jzk.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eei.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xei.jyoumei.cn

[I05] 按正则拆分
来源：http://wlg.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pnb.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lnd.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://evx.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://fdh.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://aob.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qnn.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://fsq.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uwr.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qvt.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://abm.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zir.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ils.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tbt.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dly.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tny.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://joc.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kuu.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://inr.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://owd.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bec.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mbg.fanxiaobao.xyz

TS:   /error/gim
来源：http://cng.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cnq.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ici.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://tnn.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tpj.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://lmq.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gll.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tya.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://thn.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lhv.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jas.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://khb.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ujy.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pmq.uphjek.com

================================================================================
来源：http://fui.ybcxt.top

J. 日期与时间
来源：http://tsb.jyoumei.cn

================================================================================
来源：http://jat.chenlongwang.top

[J01] 获取当前时间
来源：http://mjn.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jmi.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oaq.sweek.top

JS:   new Date();  Date.now()
来源：http://tbg.iojbl.cn

TS:   new Date();  Date.now()
来源：http://fuu.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pox.xinyue.icu

Go:   time.Now()
来源：http://usq.zhijiandao.cn

Ruby: Time.now
来源：http://bpp.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nan.haohaochexian.top

[J02] 格式化输出
来源：http://ugn.mhx1999.top


<!-- 参考信息 -->