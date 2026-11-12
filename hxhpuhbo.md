代发 wailian999

Py:   class Admin(User): pass
来源：http://umv.nwbrower.top

PHP:  class Admin extends User {}
来源：http://cfs.ywan-chungtsiang.top

JS:   class Admin extends User {}
来源：http://ajr.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://rlk.sjlbkw.cn

Java: class Admin extends User {}
来源：http://wih.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wes.chenzaomai.com

Ruby: class Admin < User; end
来源：http://trt.zhongyouzk.top

C#:   class Admin : User {}
来源：http://rps.zhongyouzk.top

[G06] 重写方法
来源：http://btf.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://mpj.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vty.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://prh.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://fmo.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://sbd.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uqx.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://fez.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://trt.jianghu66.top

[G07] 调用父类方法
来源：http://aha.0kj1m.cn

Py:   super().greet()
来源：http://bwp.tianlin.xyz

PHP:  parent::greet();
来源：http://zxu.hammf.cn

JS:   super.greet();
来源：http://pop.ywan-chungtsiang.top

TS:   super.greet();
来源：http://dij.vqdsnc.cn

Java: super.greet();
来源：http://prh.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ttn.guowangkeji.top

Ruby: super
来源：http://qjw.sjlbkw.cn

C#:   base.Greet();
来源：http://hvb.yj20258888.top

[G08] 静态方法与属性
来源：http://xzw.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hhc.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://ugn.jianghu66.top

JS:   static f() {}
来源：http://oso.zhoulong.xyz

TS:   static f(): void {}
来源：http://kbt.iojbl.cn

Java: static void f() {}
来源：http://zqo.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eim.guannengcc.top

Ruby: def self.f; end
来源：http://gyp.uphjek.com

C#:   public static void F() {}
来源：http://vxt.hesvh.cn

[G09] 接口 / 抽象类
来源：http://kji.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://keg.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tqc.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cyl.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://nwm.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://jmp.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://pdl.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ekb.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://uxa.yj20258888.top

[G10] 访问控制
来源：http://eju.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://doa.ybcxt.top

PHP:  public / protected / private
来源：http://ile.yj20258888.top

JS:   #private 字段；其余公开
来源：http://ftc.sysykeji.top

TS:   public / protected / private
来源：http://wit.ivvv.top

Java: public / protected / private / 默认包级
来源：http://lhh.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xys.ybcxt.top

Ruby: public / protected / private
来源：http://zub.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://cek.nanxuanxn.top

[G11] getter / setter
来源：http://odb.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://dkv.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dvk.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://czu.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://pcf.cashguo.top

Java: public String getName() { return name; }
来源：http://nxu.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fqw.9152youxi.cn

Ruby: attr_accessor :name
来源：http://avr.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://hlr.shzxlz.cn

[G12] 对象转字符串
来源：http://tsy.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://ovo.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://awz.yj20258888.top

JS:   toString() { return this.name; }
来源：http://sat.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://oad.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://vqe.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://hnw.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://uwj.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://wth.pengpengdd.cyou

[G13] 判断对象类型
来源：http://hud.ehwqpu.com

Py:   isinstance(u, User)
来源：http://qui.kuanghao11.cn

PHP:  $u instanceof User
来源：http://mfp.wangshuangyany.cn

JS:   u instanceof User
来源：http://tof.zhijiandao.cn

TS:   u instanceof User
来源：http://mmd.nwbrower.top

Java: u instanceof User
来源：http://dje.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vvz.cheryme.top

Ruby: u.is_a?(User)
来源：http://phy.sjlbkw.cn

C#:   u is User
来源：http://tqy.fehbvm.com

[G14] 数据类 / record
来源：http://yjr.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kjd.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://vmg.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://cnm.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://onj.ybcxt.top

Java: record User(String name, int age) {}
来源：http://rdn.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://hvw.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fwt.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://oof.fzhhl.top

[G15] 枚举
来源：http://ery.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zys.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tjd.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iog.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jep.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://yhx.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oys.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://scb.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bjs.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://chp.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wzk.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://sfy.vehdjk.com

JS:   Object.entries(obj)
来源：http://tfg.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://btp.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://twr.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xzr.0kj1m.cn

Ruby: obj.instance_variables
来源：http://ufe.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://ugi.ctjpmb.com

================================================================================
来源：http://heb.xuetiantiany.cn

H. 异常与错误处理
来源：http://zjr.jqgufenzy.top

================================================================================
来源：http://qkq.vqdsnc.cn

[H01] try / catch 基础
来源：http://opp.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://afu.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vhk.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mcr.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://omo.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://onz.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yqc.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zmo.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tkn.wangdashe.top

[H02] finally / ensure 收尾
来源：http://vxy.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://ryq.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mkf.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ncd.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://szv.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://dtz.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qub.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://orr.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://tmc.vehdjk.com

[H03] 主动抛出异常
来源：http://xau.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://omp.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://evz.tarul.cn

JS:   throw new Error("错误信息");
来源：http://mwp.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://wgc.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eng.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mxs.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://shj.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://mzb.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://hav.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://bzb.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://bvy.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://fan.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://eqs.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://duv.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dyp.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://dat.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://fsp.ctjpmb.com

[H05] 捕获特定类型
来源：http://vxb.xuanzx.com

Py:   except ValueError as e:
来源：http://ifu.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nom.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://fio.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://lhz.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://kvy.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mxc.yueranfly.top

Ruby: rescue ArgumentError => e
来源：http://zkx.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ioq.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://iru.iojbl.cn

Py:   value = d.get("k") or default
来源：http://glh.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://ext.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://wqm.shangyingyoupin.top

TS:   obj?.a?.b;  d ?? default
来源：http://wza.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dbh.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tft.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://lbv.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://paq.gaohongyu789.top

[H07] 断言
来源：http://bwm.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://fth.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://hzy.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://lkj.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://mlc.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://mmy.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rnu.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vjb.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://jmj.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://fpa.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://pbw.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rwb.guowangkeji.top

JS:   e.message;  e.stack
来源：http://nlp.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nxf.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://umb.jianghu66.top

Go:   err.Error()
来源：http://eyy.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://fow.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://oqq.uphjek.com

[H09] 带错误码的异常
来源：http://ifu.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wxx.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://bsl.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xzs.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmu.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://phq.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wpu.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://jcy.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://byr.nanxinkj.top

[H10] 资源自动释放
来源：http://zhf.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ztz.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tuv.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dzs.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yor.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vla.yj202588.top

Go:   defer f.Close()
来源：http://abe.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://obx.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rry.zdbjq.cn

================================================================================
来源：http://jif.dianchejie.cn

I. 正则表达式
来源：http://kax.redwolf501.top

================================================================================
来源：http://ide.hesvh.cn

[I01] 判断是否匹配
来源：http://dqe.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gpr.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ydp.wangdashe.top

JS:   /\d+/.test(s)
来源：http://qpk.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://gfe.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qgb.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://smc.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://how.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mag.ywan-chungtsiang.top

[I02] 提取所有匹配
来源：http://fxi.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://dta.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lme.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yfm.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://wjx.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://isk.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://muq.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://mov.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rtc.zhoulong.xyz

[I03] 提取捕获分组
来源：http://lqb.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rpi.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ads.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://khj.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vna.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jkg.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zlw.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mez.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rcm.cheryme.top

[I04] 正则替换
来源：http://oht.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fag.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wjn.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://psj.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://bwm.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://tpl.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fiw.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wpp.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hfk.yfazqb.com

[I05] 按正则拆分
来源：http://tvq.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jul.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hlh.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://cet.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://oxp.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://mwo.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pux.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://usj.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yxi.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vsg.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfr.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ecg.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krf.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xtb.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wbv.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tye.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qez.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rtj.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://aah.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cnu.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dxi.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mar.yanxiufei.cn

TS:   /error/gim
来源：http://tyt.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://svz.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mxn.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://ihf.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mfi.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://ydd.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mov.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mmv.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lvg.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpj.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gfw.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://afo.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jrx.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://auk.sweek.top

================================================================================
来源：http://vel.jlsjyb.cn

J. 日期与时间
来源：http://hab.epnwcf.com

================================================================================
来源：http://bri.ydzc1.top

[J01] 获取当前时间
来源：http://dgs.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vkw.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avu.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://nsi.cheryme.top

TS:   new Date();  Date.now()
来源：http://kgk.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lwn.ppjwa.cn

Go:   time.Now()
来源：http://gfj.aibaodan.cn

Ruby: Time.now
来源：http://ljn.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vzk.jqgufenzy.top

[J02] 格式化输出
来源：http://jqo.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rkg.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zsj.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tqe.zhengqikj.top

TS:   d.toISOString()
来源：http://yhr.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iws.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhh.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ngk.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ici.ehwqpu.com

[J03] 字符串解析为日期
来源：http://xev.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qhz.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://inj.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://wij.daria6918.cn


<!-- 参考信息 -->