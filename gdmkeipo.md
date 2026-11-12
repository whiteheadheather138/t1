代发 wailian999

Ruby: @name = "x"
来源：http://nzi.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://urd.yj20258.top

[G04] 定义方法
来源：http://gul.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://ext.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://epu.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://cxz.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://dhk.meibo888.top

Java: String greet() { return name; }
来源：http://tdb.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://qee.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://sdz.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://wjq.hnqzz.top

[G05] 继承
来源：http://myb.yongpay.top

Py:   class Admin(User): pass
来源：http://ert.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://iim.cdnleiting.top

JS:   class Admin extends User {}
来源：http://wtf.jinqigufen.top

TS:   class Admin extends User {}
来源：http://oro.nwbrower.top

Java: class Admin extends User {}
来源：http://fux.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uuh.xinyue.icu

Ruby: class Admin < User; end
来源：http://hnh.316326.xyz

C#:   class Admin : User {}
来源：http://kix.cashguo.top

[G06] 重写方法
来源：http://ejx.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://jur.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hyu.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://kzy.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://xqk.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://dzt.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dez.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://kfl.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://drc.yanxiufei.cn

[G07] 调用父类方法
来源：http://ema.jinqigufen.top

Py:   super().greet()
来源：http://zjz.vqdsnc.cn

PHP:  parent::greet();
来源：http://jeo.haohaochexian.top

JS:   super.greet();
来源：http://mjd.zhongyouzk.top

TS:   super.greet();
来源：http://iez.meibo888.top

Java: super.greet();
来源：http://oad.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://syr.ydjk.org.cn

Ruby: super
来源：http://aov.hnqzz.top

C#:   base.Greet();
来源：http://xuz.jinqigufen.top

[G08] 静态方法与属性
来源：http://mrf.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oey.nwbrower.top

PHP:  public static function f() {}
来源：http://wxo.sweek.top

JS:   static f() {}
来源：http://uyy.yongpay.top

TS:   static f(): void {}
来源：http://brr.zhixingplan.top

Java: static void f() {}
来源：http://fyk.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iui.ydjk.org.cn

Ruby: def self.f; end
来源：http://wsw.yangfankeji.com

C#:   public static void F() {}
来源：http://fdm.sweek.top

[G09] 接口 / 抽象类
来源：http://qqa.shuidangran.top

Py:   from abc import ABC, abstractmethod
来源：http://out.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://jau.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jdr.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://doy.mhx1999.top

Java: interface Shape { double area(); }
来源：http://odp.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://spx.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gov.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://dxg.xinyue.icu

[G10] 访问控制
来源：http://keu.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://ywq.hongshengwenyu.top

PHP:  public / protected / private
来源：http://yzy.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://xmn.ppjwa.cn

TS:   public / protected / private
来源：http://dlx.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://nbq.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ksu.cheryme.top

Ruby: public / protected / private
来源：http://dgz.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://clf.shanyushiyangkeji.top

[G11] getter / setter
来源：http://hxr.xylfe.cn

Py:   @property 与 @x.setter
来源：http://bdx.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mnm.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://ppc.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://scy.cheryme.top

Java: public String getName() { return name; }
来源：http://fkg.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbd.fengsongda.top

Ruby: attr_accessor :name
来源：http://nle.cashguo.top

C#:   public string Name { get; set; }
来源：http://dro.hnxiangtu.top

[G12] 对象转字符串
来源：http://ixh.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://ebm.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fvi.guannengcc.top

JS:   toString() { return this.name; }
来源：http://gou.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://eeb.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://wml.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://zhn.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://udy.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://rmq.epnwcf.com

[G13] 判断对象类型
来源：http://zjx.mhx1999.top

Py:   isinstance(u, User)
来源：http://vft.yongpay.top

PHP:  $u instanceof User
来源：http://jwk.hesvh.cn

JS:   u instanceof User
来源：http://tud.dianchejie.cn

TS:   u instanceof User
来源：http://plw.cucudq.cn

Java: u instanceof User
来源：http://msw.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsk.zhixingplan.top

Ruby: u.is_a?(User)
来源：http://smd.hongshengwenyu.top

C#:   u is User
来源：http://stn.hcnkem.com

[G14] 数据类 / record
来源：http://ire.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kgl.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://vxk.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://zqd.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://rad.316326.xyz

Java: record User(String name, int age) {}
来源：http://qaq.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://yxh.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://agw.hammf.cn

C#:   record User(string Name, int Age);
来源：http://vus.yj20258.top

[G15] 枚举
来源：http://nzd.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qwx.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lex.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pzf.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npe.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://vnn.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pjy.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://mav.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ymy.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://vtu.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xkx.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://xmn.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://qcp.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://cqc.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ysa.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://blh.aibaodan.cn

Ruby: obj.instance_variables
来源：http://yvd.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://sjz.hfpthk.cn

================================================================================
来源：http://zpg.gogol.net.cn

H. 异常与错误处理
来源：http://sar.zhaomingkeji.xyz

================================================================================
来源：http://lau.redwolf501.top

[H01] try / catch 基础
来源：http://lpd.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pcp.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ffj.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zoz.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qqi.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eto.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uhv.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://raf.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsa.fktsv.cn

[H02] finally / ensure 收尾
来源：http://awm.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sji.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mpo.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xfl.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kou.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://kus.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mhu.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ffw.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lqw.gaohongyu789.top

[H03] 主动抛出异常
来源：http://tdb.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://ngi.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gyz.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://qpk.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://qvl.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lew.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hkp.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://tex.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dod.tanke756.top

[H04] 自定义异常类型
来源：http://cva.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://fgj.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://onh.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://xja.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://gzz.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://myj.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sql.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://uoz.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://wql.zhongyouzk.top

[H05] 捕获特定类型
来源：http://ydv.yuxming.cn

Py:   except ValueError as e:
来源：http://stw.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mwt.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ivd.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ygj.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://pxd.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ilo.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://brk.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cqt.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://bbf.yongpay.top

Py:   value = d.get("k") or default
来源：http://mfh.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wgn.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://qgs.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://rjw.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vry.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://plk.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://rjh.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://hon.jqgfzy.top

[H07] 断言
来源：http://uqg.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://vrp.nwbrower.top

PHP:  assert($x > 0);
来源：http://xbw.mhx1999.top

JS:   console.assert(x > 0);
来源：http://pxs.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://irj.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://vqx.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bnt.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://iro.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://ffk.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://pxa.ehwqpu.com

Py:   str(e);  traceback.format_exc()
来源：http://yld.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rph.52xcode.cn

JS:   e.message;  e.stack
来源：http://dtp.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tdx.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://cnn.redwolf501.top

Go:   err.Error()
来源：http://edq.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://acn.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://zne.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://jil.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xnm.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://riy.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sgj.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xrn.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://moj.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iri.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://uvt.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yuq.hnxiangtu.top

[H10] 资源自动释放
来源：http://tpd.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://quv.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wil.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dbc.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wnt.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mav.wangshuangyany.cn

Go:   defer f.Close()
来源：http://crg.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qlp.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aes.cdnleiting.top

================================================================================
来源：http://dmx.ivvv.top

I. 正则表达式
来源：http://mjw.sufxvd.cn

================================================================================
来源：http://esa.jyoumei.cn

[I01] 判断是否匹配
来源：http://nyf.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://woz.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rae.hesvh.cn

JS:   /\d+/.test(s)
来源：http://ehw.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://qjm.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://elv.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jau.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://hde.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bwd.gzhubu.top

[I02] 提取所有匹配
来源：http://xpq.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://nlz.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hsj.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xrt.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://dmk.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://emk.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fkh.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://wky.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqp.hesvh.cn

[I03] 提取捕获分组
来源：http://eau.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kov.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ynh.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ubt.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uqs.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ftg.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gto.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yie.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ial.yangfankeji.com

[I04] 正则替换
来源：http://nwz.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mme.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vdy.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://qmz.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://unz.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://cas.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sla.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lkl.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byo.jyoumei.cn

[I05] 按正则拆分
来源：http://ymy.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xgn.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cwm.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://xmn.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://adf.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://wym.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nmy.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://ikv.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hau.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iwg.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wig.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fui.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdm.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mrk.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cob.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yfj.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://los.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fbk.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://bau.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://onm.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zyu.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wfn.sweek.top

TS:   /error/gim
来源：http://dkn.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wja.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gzx.yonumen.top

Ruby: s.scan(/error/i)
来源：http://dxz.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdi.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://mct.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iav.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ift.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bmx.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfi.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sxb.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ujy.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iho.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kqb.shangyingyoupin.top

================================================================================
来源：http://xfe.ydjk.org.cn

J. 日期与时间
来源：http://dok.uphjek.com

================================================================================
来源：http://glx.cucudq.cn

[J01] 获取当前时间
来源：http://xke.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://hfs.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dbi.sysykeji.top

JS:   new Date();  Date.now()
来源：http://fqv.hcnkem.com

TS:   new Date();  Date.now()
来源：http://dhx.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ejt.sweek.top

Go:   time.Now()
来源：http://tyt.vehdjk.com

Ruby: Time.now
来源：http://ikw.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tie.yongpay.top

[J02] 格式化输出
来源：http://gye.yfazqb.com


<!-- 参考信息 -->