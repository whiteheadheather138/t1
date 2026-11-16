代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://yhe.cdnleiting.top

Ruby: def greet; @name; end
来源：http://stm.tarul.cn

C#:   public string Greet() => Name;
来源：http://wwd.cashguo.top

[G05] 继承
来源：http://uwk.hfpthk.cn

Py:   class Admin(User): pass
来源：http://hzz.52xcode.cn

PHP:  class Admin extends User {}
来源：http://vub.c1oappe.top

JS:   class Admin extends User {}
来源：http://euh.zhengqikj.top

TS:   class Admin extends User {}
来源：http://kev.vehdjk.com

Java: class Admin extends User {}
来源：http://bnm.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rcz.nanxinkj.top

Ruby: class Admin < User; end
来源：http://sau.zhixingplan.top

C#:   class Admin : User {}
来源：http://lyn.smart0.xyz

[G06] 重写方法
来源：http://xcd.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://mda.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tih.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://cnl.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://xok.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://kyw.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dic.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://hgp.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://dwp.fzhhl.top

[G07] 调用父类方法
来源：http://wya.aizwys.cn

Py:   super().greet()
来源：http://ivn.chenzaomai.com

PHP:  parent::greet();
来源：http://mmn.ppjwa.cn

JS:   super.greet();
来源：http://gli.jiagoushi.top

TS:   super.greet();
来源：http://vwc.meibo888.top

Java: super.greet();
来源：http://ksl.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wei.andypj.xyz

Ruby: super
来源：http://dmh.shuidangran.top

C#:   base.Greet();
来源：http://scy.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://jdo.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ghh.snrcjt.cn

PHP:  public static function f() {}
来源：http://mdf.uphjek.com

JS:   static f() {}
来源：http://izv.tanke756.top

TS:   static f(): void {}
来源：http://kof.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://ucl.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jqj.ppjwa.cn

Ruby: def self.f; end
来源：http://cnn.hammf.cn

C#:   public static void F() {}
来源：http://ptg.xuanzx.com

[G09] 接口 / 抽象类
来源：http://rxa.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://exw.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://rmd.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kvp.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://cig.zycfv.cn

Java: interface Shape { double area(); }
来源：http://vgc.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://ckf.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qvk.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://pwq.chenzaomai.com

[G10] 访问控制
来源：http://ikv.yuanzhike.top

Py:   约定 _protected / __private（不强制）
来源：http://bry.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://vhz.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://bhe.xziqi.cn

TS:   public / protected / private
来源：http://lpw.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://lqb.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ntf.chenjidiqi.icu

Ruby: public / protected / private
来源：http://gkj.cheryme.top

C#:   public / protected / private / internal
来源：http://nxt.aizwys.cn

[G11] getter / setter
来源：http://une.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://xjq.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jse.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://txn.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://ptm.yj20258888.top

Java: public String getName() { return name; }
来源：http://vol.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lkg.fehbvm.com

Ruby: attr_accessor :name
来源：http://aob.hcnkem.com

C#:   public string Name { get; set; }
来源：http://far.snrcjt.cn

[G12] 对象转字符串
来源：http://wmh.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://psz.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://otr.nwbrower.top

JS:   toString() { return this.name; }
来源：http://xha.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://vtw.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://wmj.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://sds.smart0.xyz

Ruby: def to_s; @name; end
来源：http://auv.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://aaz.jqgufenzy.top

[G13] 判断对象类型
来源：http://fsk.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://ovl.hnqzz.top

PHP:  $u instanceof User
来源：http://lap.jyoumei.cn

JS:   u instanceof User
来源：http://kni.zhixingplan.top

TS:   u instanceof User
来源：http://xgz.chenlongwang.top

Java: u instanceof User
来源：http://etr.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kej.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://rpo.gzhubu.top

C#:   u is User
来源：http://xwd.jlsjyb.cn

[G14] 数据类 / record
来源：http://wjh.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pdr.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://fuk.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://edo.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://gnu.daria6918.cn

Java: record User(String name, int age) {}
来源：http://tzb.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://jhn.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hor.jiagoushi.top

C#:   record User(string Name, int Age);
来源：http://pny.hysaishi.cn

[G15] 枚举
来源：http://ims.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mpk.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://apc.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fqu.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sak.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://bns.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://weq.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://jwb.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bsd.cashguo.top

[G16] 对象转数组 / 字典
来源：http://jgu.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zzz.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://kqb.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://dnf.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://bye.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vkj.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hxs.hnqzz.top

Ruby: obj.instance_variables
来源：http://khx.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://jax.xylfe.cn

================================================================================
来源：http://vqt.hesvh.cn

H. 异常与错误处理
来源：http://mzr.ydzc1.top

================================================================================
来源：http://ixg.nanxinkj.top

[H01] try / catch 基础
来源：http://euh.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrv.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nyo.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kww.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zrp.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ayc.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mli.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jvg.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qnm.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://lqb.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gnf.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xcp.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qua.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xxw.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://fwo.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://gcw.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rrn.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://lht.uphjek.com

[H03] 主动抛出异常
来源：http://rlp.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://kyj.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yhl.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://kyk.meibo888.top

TS:   throw new Error("错误信息");
来源：http://gur.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xjz.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yga.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dyg.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://iwm.svipenyu.cn

[H04] 自定义异常类型
来源：http://gdp.yongpay.top

Py:   class MyError(Exception): pass
来源：http://ism.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yhp.cashguo.top

JS:   class MyError extends Error {}
来源：http://fcu.xylfe.cn

TS:   class MyError extends Error {}
来源：http://gaz.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://fpp.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://htz.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://pen.dianchejie.cn

C#:   class MyException : Exception {}
来源：http://bal.quarkkingdee.top

[H05] 捕获特定类型
来源：http://bvm.zdbjq.cn

Py:   except ValueError as e:
来源：http://sds.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hhe.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://cay.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://apn.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://kao.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hir.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://zgv.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qyf.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://bvs.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://hcn.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vxt.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tlh.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zak.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yfg.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://iip.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://tdf.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://onh.haohaochexian.top

[H07] 断言
来源：http://qch.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://xin.zycfv.cn

PHP:  assert($x > 0);
来源：http://xfk.sxryk.cn

JS:   console.assert(x > 0);
来源：http://pwd.epnwcf.com

TS:   console.assert(x > 0);
来源：http://dqm.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://buo.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lrx.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://tba.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://qut.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://qby.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://fyu.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbc.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://tpk.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vjl.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ess.zhixingplan.top

Go:   err.Error()
来源：http://blt.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://prm.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://lko.jqgufenzy.top

[H09] 带错误码的异常
来源：http://ehn.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dkn.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kfo.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wwt.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nfk.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ngx.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nev.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://enx.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ung.gotoacloud.top

[H10] 资源自动释放
来源：http://zlj.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://fsw.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oap.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://air.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bbp.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gfc.yj20258.top

Go:   defer f.Close()
来源：http://swt.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vjd.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jvl.hywenlv.cn

================================================================================
来源：http://bof.xylfe.cn

I. 正则表达式
来源：http://nvk.guannengcc.top

================================================================================
来源：http://yfx.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://jci.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gfv.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://bkm.52xcode.cn

JS:   /\d+/.test(s)
来源：http://gfg.ydzc1.top

TS:   /\d+/.test(s)
来源：http://cvr.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uqu.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uge.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://vkf.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ukp.andypj.xyz

[I02] 提取所有匹配
来源：http://xsf.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://eln.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sfl.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lkg.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://vhp.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fix.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uyh.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://tjd.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zjz.0kj1m.cn

[I03] 提取捕获分组
来源：http://nso.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pdy.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://clc.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zlh.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lyo.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oga.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uss.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vey.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kqh.guowangkeji.top

[I04] 正则替换
来源：http://ohy.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://llz.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pac.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://luc.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://rrr.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://csw.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://xjb.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xws.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ikw.sufxvd.cn

[I05] 按正则拆分
来源：http://uwn.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://rns.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tae.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://afa.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://fqr.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://hej.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jge.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zuk.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pki.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://atn.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ymo.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://urw.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpt.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wip.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xhn.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bpn.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tss.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lxi.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://kfi.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eqn.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vdj.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qgp.chenzaomai.com

TS:   /error/gim
来源：http://spv.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eoj.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yhw.cashguo.top

Ruby: s.scan(/error/i)
来源：http://zsu.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mry.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://usd.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bvo.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wpe.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://euf.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pkp.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zbc.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtl.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://igr.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wlk.fengsongda.top

================================================================================
来源：http://dtr.zhixingplan.top

J. 日期与时间
来源：http://exy.sweek.top

================================================================================
来源：http://uyx.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://hjz.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cyt.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mhj.shuidangran.top

JS:   new Date();  Date.now()
来源：http://fqa.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://mdp.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uml.jlsjyb.cn

Go:   time.Now()
来源：http://rkc.aizwys.cn

Ruby: Time.now
来源：http://vdp.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mlm.nanxuanxn.top

[J02] 格式化输出
来源：http://xvc.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frb.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dhl.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bkh.cucudq.cn

TS:   d.toISOString()
来源：http://aqk.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bsl.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sue.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://exd.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nja.ybcxt.top


<!-- 参考信息 -->