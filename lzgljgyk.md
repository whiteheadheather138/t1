代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://gvu.cqqwz.cn

Ruby: def greet; @name; end
来源：http://fsl.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://mcw.vehdjk.com

[G05] 继承
来源：http://rvu.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://anu.daxiang520.top

PHP:  class Admin extends User {}
来源：http://iwa.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://tok.fktsv.cn

TS:   class Admin extends User {}
来源：http://vkx.gaohongyu789.top

Java: class Admin extends User {}
来源：http://qen.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lyc.smart0.xyz

Ruby: class Admin < User; end
来源：http://mhh.tianlin.xyz

C#:   class Admin : User {}
来源：http://acr.ybcxt.top

[G06] 重写方法
来源：http://aho.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://ujt.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://knf.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://hnw.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://vrx.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://vft.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lla.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://vpj.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://wrp.aibaodan.cn

[G07] 调用父类方法
来源：http://lmz.feifeiyinyue.top

Py:   super().greet()
来源：http://bgi.snrcjt.cn

PHP:  parent::greet();
来源：http://lco.jianghu66.top

JS:   super.greet();
来源：http://vbo.jyoumei.cn

TS:   super.greet();
来源：http://man.feifeiyinyue.top

Java: super.greet();
来源：http://hjf.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hbk.zhixingplan.top

Ruby: super
来源：http://ofl.yonumen.top

C#:   base.Greet();
来源：http://xsf.fzhhl.top

[G08] 静态方法与属性
来源：http://hoc.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://saf.cqqwz.cn

PHP:  public static function f() {}
来源：http://ehg.uphjek.com

JS:   static f() {}
来源：http://pyo.ivvv.top

TS:   static f(): void {}
来源：http://tdq.epnwcf.com

Java: static void f() {}
来源：http://bjl.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kyd.feifeiyinyue.top

Ruby: def self.f; end
来源：http://uxl.gaohongyu789.top

C#:   public static void F() {}
来源：http://aim.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://kle.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://yve.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://err.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lks.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://vno.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://xar.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://vyu.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vsd.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://olj.cashguo.top

[G10] 访问控制
来源：http://cbw.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://ups.jyoumei.cn

PHP:  public / protected / private
来源：http://xyc.wangdashe.top

JS:   #private 字段；其余公开
来源：http://mua.sweek.top

TS:   public / protected / private
来源：http://cjd.ivvv.top

Java: public / protected / private / 默认包级
来源：http://hqw.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://srz.xuanzx.com

Ruby: public / protected / private
来源：http://pxu.hcnkem.com

C#:   public / protected / private / internal
来源：http://any.meibo888.top

[G11] getter / setter
来源：http://ahh.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://wse.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qdy.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://mqa.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://sjq.yvedp.cn

Java: public String getName() { return name; }
来源：http://zbm.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ftj.xylfe.cn

Ruby: attr_accessor :name
来源：http://njw.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://bcf.havefunace.top

[G12] 对象转字符串
来源：http://oiw.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://fyw.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ncu.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://ghm.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://gdm.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://bmn.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jwj.mhx1999.top

Ruby: def to_s; @name; end
来源：http://end.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://qly.meibo888.top

[G13] 判断对象类型
来源：http://ujm.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://mie.redwolf501.top

PHP:  $u instanceof User
来源：http://yfy.gogol.net.cn

JS:   u instanceof User
来源：http://pmy.birdmap.top

TS:   u instanceof User
来源：http://thg.hammf.cn

Java: u instanceof User
来源：http://kdx.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ogc.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://iwt.jianghu66.top

C#:   u is User
来源：http://mom.hnqzz.top

[G14] 数据类 / record
来源：http://bsd.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iib.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://bxf.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://vcr.cdnleiting.top

TS:   type User = { name: string; age: number };
来源：http://jla.daxiang520.top

Java: record User(String name, int age) {}
来源：http://fwp.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://uaq.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pzo.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://ldj.yvedp.cn

[G15] 枚举
来源：http://sra.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fag.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ddx.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ncu.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gwz.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://yfq.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cje.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://pfw.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jof.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://uly.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://djq.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://bsa.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://cwb.fzhhl.top

TS:   Object.entries(obj)
来源：http://mzt.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://snm.fktsv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qsu.yuanzhike.top

Ruby: obj.instance_variables
来源：http://jve.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://clg.vehdjk.com

================================================================================
来源：http://yya.hfpthk.cn

H. 异常与错误处理
来源：http://wwj.chenzaomai.com

================================================================================
来源：http://mkw.yj202588.top

[H01] try / catch 基础
来源：http://uvr.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gnf.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efj.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nsa.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jba.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://abi.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gec.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fwf.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://umg.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://wem.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gob.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://adz.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iwg.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lct.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ocp.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zhg.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vor.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjz.jinqigufen.top

[H03] 主动抛出异常
来源：http://emk.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://wws.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yca.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://oym.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://rma.sysykeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ftq.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://loy.zdbjq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fpb.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://iai.ctjpmb.com

[H04] 自定义异常类型
来源：http://omq.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://fgp.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://lyx.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://kbg.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://usm.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://tpq.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kfc.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://foy.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://umd.tarul.cn

[H05] 捕获特定类型
来源：http://ple.zdbjq.cn

Py:   except ValueError as e:
来源：http://wqr.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qha.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://nna.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://nmg.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://awj.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qpg.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://qdn.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cei.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://wnt.bjfxy.top

Py:   value = d.get("k") or default
来源：http://exn.sysykeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://tov.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://mkd.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hhk.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ksp.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xtb.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://uol.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://hvo.jinqigfzy.top

[H07] 断言
来源：http://kyd.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://vka.snrcjt.cn

PHP:  assert($x > 0);
来源：http://nmh.xylfe.cn

JS:   console.assert(x > 0);
来源：http://rvz.gzhubu.top

TS:   console.assert(x > 0);
来源：http://fdv.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://qfk.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndo.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://dsv.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://cru.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://fox.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://myg.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hrb.mhx1999.top

JS:   e.message;  e.stack
来源：http://pqb.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mzf.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://psx.yvedp.cn

Go:   err.Error()
来源：http://gic.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://xfr.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://xyg.yueranfly.top

[H09] 带错误码的异常
来源：http://dmr.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xoq.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wnl.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yzh.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pnk.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rhh.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tzx.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://pfs.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fbz.wangdashe.top

[H10] 资源自动释放
来源：http://rvn.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xgo.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xah.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qkx.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mjl.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uut.tianlin.xyz

Go:   defer f.Close()
来源：http://iab.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dlh.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mup.pycfn.com

================================================================================
来源：http://cyv.yueranfly.top

I. 正则表达式
来源：http://fcc.tarul.cn

================================================================================
来源：http://goh.jqgufenzy.top

[I01] 判断是否匹配
来源：http://wvm.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vbm.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://uur.fktsv.cn

JS:   /\d+/.test(s)
来源：http://ziz.vehdjk.com

TS:   /\d+/.test(s)
来源：http://wuy.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bax.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dwd.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://xrx.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zop.nanxuanxn.top

[I02] 提取所有匹配
来源：http://jbp.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://vvb.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fqj.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vgj.uphjek.com

TS:   s.match(/\d+/g)
来源：http://ggs.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zve.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://moc.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://pam.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikm.hysaishi.cn

[I03] 提取捕获分组
来源：http://fun.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fic.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://igk.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dck.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qhv.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zht.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gxn.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gkw.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://itd.nanxuanxn.top

[I04] 正则替换
来源：http://pcw.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pki.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iqv.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eln.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gan.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qud.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qdb.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tjp.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qne.xuetiantiany.cn

[I05] 按正则拆分
来源：http://nxx.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zas.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://umd.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://mfj.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://lbb.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://uwm.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gtn.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://ndo.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://klq.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gtj.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rpj.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://coh.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://irs.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xjm.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tzy.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kpk.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zcm.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yku.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://duo.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qpf.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rgc.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ate.ppjwa.cn

TS:   /error/gim
来源：http://rpl.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ndz.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://djf.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://bby.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jct.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://ljo.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nja.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vyc.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqk.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jzq.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wna.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ycs.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lan.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zhx.quarkkingdee.top

================================================================================
来源：http://sti.hesvh.cn

J. 日期与时间
来源：http://cgm.meibo888.top

================================================================================
来源：http://sni.sysykeji.top

[J01] 获取当前时间
来源：http://rel.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nnw.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://usg.sweek.top

JS:   new Date();  Date.now()
来源：http://xso.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://vsc.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://iwh.ydjk.org.cn

Go:   time.Now()
来源：http://irp.ivvv.top

Ruby: Time.now
来源：http://ssd.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pfr.fanxiaobao.xyz

[J02] 格式化输出
来源：http://lup.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xqn.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pko.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://asi.yuanzhike.top

TS:   d.toISOString()
来源：http://nka.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aay.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fzs.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zxe.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ixz.fengsongda.top


<!-- 参考信息 -->