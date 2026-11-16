代发 wailian999

Ruby: @name = "x"
来源：http://kly.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://qol.tian-w.cn

[G04] 定义方法
来源：http://bng.yongpay.top

Py:   def greet(self): return self.name
来源：http://vfl.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pqr.yuxming.cn

JS:   greet() { return this.name; }
来源：http://sil.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://clr.xinyue.icu

Java: String greet() { return name; }
来源：http://pdc.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mxc.cqqwz.cn

Ruby: def greet; @name; end
来源：http://phy.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://qjd.zhixingplan.top

[G05] 继承
来源：http://xay.xuanzx.com

Py:   class Admin(User): pass
来源：http://ueu.fktsv.cn

PHP:  class Admin extends User {}
来源：http://pqz.chenzaomai.com

JS:   class Admin extends User {}
来源：http://ozj.uphjek.com

TS:   class Admin extends User {}
来源：http://tft.bbcook.cn

Java: class Admin extends User {}
来源：http://bqa.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ehs.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://hgq.tanke756.top

C#:   class Admin : User {}
来源：http://tix.yj20258888.top

[G06] 重写方法
来源：http://xhq.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://kbc.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://pxe.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://nel.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://ome.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://aza.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rch.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://kzz.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://lfn.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://wok.yueranfly.top

Py:   super().greet()
来源：http://myp.xinyue.icu

PHP:  parent::greet();
来源：http://rer.shuidangran.top

JS:   super.greet();
来源：http://vax.aizwys.cn

TS:   super.greet();
来源：http://oqa.daxiang520.top

Java: super.greet();
来源：http://lpt.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ziu.cucudq.cn

Ruby: super
来源：http://crm.nwbrower.top

C#:   base.Greet();
来源：http://wuz.hywenlv.cn

[G08] 静态方法与属性
来源：http://sxe.dashuyun.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esx.svipenyu.cn

PHP:  public static function f() {}
来源：http://lef.jianghu66.top

JS:   static f() {}
来源：http://cls.kuanghao11.cn

TS:   static f(): void {}
来源：http://zai.0kj1m.cn

Java: static void f() {}
来源：http://pxa.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ted.jqgufenzy.top

Ruby: def self.f; end
来源：http://hlu.ppjwa.cn

C#:   public static void F() {}
来源：http://clg.ywan-chungtsiang.top

[G09] 接口 / 抽象类
来源：http://xmh.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://kpz.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://mee.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qks.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://dqa.bbcook.cn

Java: interface Shape { double area(); }
来源：http://ees.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://bmy.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wcj.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://yqs.fktsv.cn

[G10] 访问控制
来源：http://lsw.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://ukj.yj20258.top

PHP:  public / protected / private
来源：http://cbr.sysykeji.top

JS:   #private 字段；其余公开
来源：http://bcu.yuxming.cn

TS:   public / protected / private
来源：http://wgh.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://zmd.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qzi.sjlbkw.cn

Ruby: public / protected / private
来源：http://txk.tanke756.top

C#:   public / protected / private / internal
来源：http://bad.guowangkeji.top

[G11] getter / setter
来源：http://iws.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://tfo.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pje.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://lie.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://xxj.guowangkeji.top

Java: public String getName() { return name; }
来源：http://dvr.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://emv.havefunace.top

Ruby: attr_accessor :name
来源：http://nfy.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://zgf.yuxming.cn

[G12] 对象转字符串
来源：http://dse.birdmap.top

Py:   def __str__(self): return self.name
来源：http://ubs.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bje.c1oappe.top

JS:   toString() { return this.name; }
来源：http://mzk.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://iky.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://mnh.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://kml.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://ykz.sweek.top

C#:   public override string ToString() => Name;
来源：http://pdp.gogol.net.cn

[G13] 判断对象类型
来源：http://xnn.gogol.net.cn

Py:   isinstance(u, User)
来源：http://irh.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://vcx.xinyue.icu

JS:   u instanceof User
来源：http://sfg.aizwys.cn

TS:   u instanceof User
来源：http://jqa.sysykeji.top

Java: u instanceof User
来源：http://vyf.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkz.yfazqb.com

Ruby: u.is_a?(User)
来源：http://drl.sweek.top

C#:   u is User
来源：http://sny.52xcode.cn

[G14] 数据类 / record
来源：http://tmn.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hhy.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://gyt.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vle.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://gam.hesvh.cn

Java: record User(String name, int age) {}
来源：http://llp.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://npf.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blc.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://hti.0kj1m.cn

[G15] 枚举
来源：http://aqq.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jbn.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://csx.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qzz.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tbn.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://uyq.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eik.chenjidiqi.icu

Ruby: Color = %i[red green].freeze
来源：http://oik.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rnt.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://mny.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fth.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://cwm.zhengqikj.top

JS:   Object.entries(obj)
来源：http://imy.fengsongda.top

TS:   Object.entries(obj)
来源：http://sug.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nmf.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lkp.guowangkeji.top

Ruby: obj.instance_variables
来源：http://avr.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://tzz.yanxiufei.cn

================================================================================
来源：http://htx.zhoulong.xyz

H. 异常与错误处理
来源：http://oay.shangyingyoupin.top

================================================================================
来源：http://hur.yj20258888.top

[H01] try / catch 基础
来源：http://sod.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blw.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bsz.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mtj.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://max.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rti.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rmi.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vpa.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xjy.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://xpw.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yse.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://orn.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xqi.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xow.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wzg.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lua.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pim.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kul.yonumen.top

[H03] 主动抛出异常
来源：http://tak.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://oay.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tib.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://vvz.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://oer.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sxb.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hcf.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hqy.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://jgu.zycfv.cn

[H04] 自定义异常类型
来源：http://djn.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://dkl.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aay.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://lph.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://dfe.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://aug.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dsw.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://xzl.bjfxy.top

C#:   class MyException : Exception {}
来源：http://kdu.zycfv.cn

[H05] 捕获特定类型
来源：http://gfh.cucudq.cn

Py:   except ValueError as e:
来源：http://jkf.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yok.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://dfc.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://tyl.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://eiy.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lto.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://pmt.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://obd.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://piq.smart0.xyz

Py:   value = d.get("k") or default
来源：http://xyd.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://chw.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://rmh.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uuy.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jmu.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xbp.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://crd.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://xbs.meibo888.top

[H07] 断言
来源：http://djx.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://xht.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://ikk.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://hbw.daxiang520.top

TS:   console.assert(x > 0);
来源：http://ygs.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://smx.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://npp.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://pxg.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://ais.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://iyr.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://onx.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lnl.zhengqikj.top

JS:   e.message;  e.stack
来源：http://gmz.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfl.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hbw.ppjwa.cn

Go:   err.Error()
来源：http://egd.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://sci.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://gvw.iojbl.cn

[H09] 带错误码的异常
来源：http://rsd.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nmd.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ndw.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mbh.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vjd.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://unw.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wpk.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://xox.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xtg.gogol.net.cn

[H10] 资源自动释放
来源：http://jwg.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qio.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ijn.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ouz.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://flz.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rvb.dashuyun.cn

Go:   defer f.Close()
来源：http://izw.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bzw.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wqp.0kj1m.cn

================================================================================
来源：http://yfn.jqgufenzy.top

I. 正则表达式
来源：http://fjb.ctjpmb.com

================================================================================
来源：http://qzd.gaohongyu789.top

[I01] 判断是否匹配
来源：http://pvn.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ois.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://hlr.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://rdj.cheryme.top

TS:   /\d+/.test(s)
来源：http://rkw.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kvq.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jch.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://qpn.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://luf.birdmap.top

[I02] 提取所有匹配
来源：http://piw.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://ely.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gso.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qah.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://omu.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vfj.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qzb.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://gce.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yrd.hysaishi.cn

[I03] 提取捕获分组
来源：http://fem.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ayq.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qax.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://orp.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cni.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yes.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vmm.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbk.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pzs.tanke756.top

[I04] 正则替换
来源：http://amf.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://csv.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://onr.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xxr.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://gvp.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://ivz.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gqw.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://npg.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwc.nwbrower.top

[I05] 按正则拆分
来源：http://iqk.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mrb.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exl.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://ity.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://equ.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://osd.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ula.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://fzi.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hdy.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bkw.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ufq.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://biy.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebf.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mcb.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tie.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wtj.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zjn.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gad.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://mvm.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://map.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qmh.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://snx.ybcxt.top

TS:   /error/gim
来源：http://law.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kjg.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uwq.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://gxo.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tjs.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://khi.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gaa.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://odb.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tbn.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jiw.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sml.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fvd.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jsp.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uxy.zhiwuduotai.top

================================================================================
来源：http://dyq.xuanzx.com

J. 日期与时间
来源：http://ucc.cdnleiting.top

================================================================================
来源：http://gwi.yueranfly.top

[J01] 获取当前时间
来源：http://uww.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://czm.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsd.yj202588.top

JS:   new Date();  Date.now()
来源：http://xvn.smart0.xyz

TS:   new Date();  Date.now()
来源：http://ihc.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dki.jyoumei.cn

Go:   time.Now()
来源：http://owt.tianlin.xyz

Ruby: Time.now
来源：http://trl.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pjm.tianlin.xyz

[J02] 格式化输出
来源：http://vhs.ydjk.org.cn


<!-- 参考信息 -->