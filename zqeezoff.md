代发 wailian999

Ruby: @name = "x"
来源：http://mcj.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vvy.aibaodan.cn

[G04] 定义方法
来源：http://ngf.havefunace.top

Py:   def greet(self): return self.name
来源：http://hxa.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://kjw.tarul.cn

JS:   greet() { return this.name; }
来源：http://gfg.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://qxy.sweek.top

Java: String greet() { return name; }
来源：http://vhb.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://jdz.shzxlz.cn

Ruby: def greet; @name; end
来源：http://ozk.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://ilw.aizwys.cn

[G05] 继承
来源：http://uzs.wangdashe.top

Py:   class Admin(User): pass
来源：http://jan.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://oxi.jqgfzy.top

JS:   class Admin extends User {}
来源：http://toy.gotoacloud.top

TS:   class Admin extends User {}
来源：http://ifz.tarul.cn

Java: class Admin extends User {}
来源：http://hdl.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gyb.ivvv.top

Ruby: class Admin < User; end
来源：http://ivb.ctjpmb.com

C#:   class Admin : User {}
来源：http://kpo.cqqwz.cn

[G06] 重写方法
来源：http://agw.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://iks.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hrw.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://eio.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://wrc.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://wye.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tji.havefunace.top

Ruby: def greet; "admin"; end
来源：http://ftl.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://yfz.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://kgb.ctjpmb.com

Py:   super().greet()
来源：http://eoa.zhiwuduotai.top

PHP:  parent::greet();
来源：http://wkj.nwbrower.top

JS:   super.greet();
来源：http://jqu.andypj.xyz

TS:   super.greet();
来源：http://nbu.svipenyu.cn

Java: super.greet();
来源：http://ska.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bvt.c1oappe.top

Ruby: super
来源：http://sxu.quarkkingdee.top

C#:   base.Greet();
来源：http://ozi.fengsongda.top

[G08] 静态方法与属性
来源：http://ypm.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ijw.guannengcc.top

PHP:  public static function f() {}
来源：http://rtq.yuanzhike.top

JS:   static f() {}
来源：http://rfs.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://tof.quarkkingdee.top

Java: static void f() {}
来源：http://jew.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mmd.tarul.cn

Ruby: def self.f; end
来源：http://bac.guowangkeji.top

C#:   public static void F() {}
来源：http://lmz.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://sho.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://qus.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://oje.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://snu.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://vpt.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://ukj.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://cyu.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nql.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://mzm.cheryme.top

[G10] 访问控制
来源：http://ork.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://vce.cheryme.top

PHP:  public / protected / private
来源：http://zsv.epnwcf.com

JS:   #private 字段；其余公开
来源：http://qry.andypj.xyz

TS:   public / protected / private
来源：http://grf.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://utc.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pxr.bbcook.cn

Ruby: public / protected / private
来源：http://ojh.meibo888.top

C#:   public / protected / private / internal
来源：http://lku.dashuyun.cn

[G11] getter / setter
来源：http://dzo.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://lmm.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gev.bbcook.cn

JS:   get name() { return this._name; }
来源：http://fxu.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://vjq.daria6918.cn

Java: public String getName() { return name; }
来源：http://kjl.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bpy.dashuyun.cn

Ruby: attr_accessor :name
来源：http://ueg.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://ghd.redwolf501.top

[G12] 对象转字符串
来源：http://rqc.meibo888.top

Py:   def __str__(self): return self.name
来源：http://lua.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wqq.meibo888.top

JS:   toString() { return this.name; }
来源：http://ydi.sweek.top

TS:   toString(): string { return this.name; }
来源：http://lrm.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://ikp.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jcy.yueranfly.top

Ruby: def to_s; @name; end
来源：http://kwz.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://pjr.hfpthk.cn

[G13] 判断对象类型
来源：http://adg.ppjwa.cn

Py:   isinstance(u, User)
来源：http://dry.uphjek.com

PHP:  $u instanceof User
来源：http://xxr.zycfv.cn

JS:   u instanceof User
来源：http://zjc.fzhhl.top

TS:   u instanceof User
来源：http://izi.kuanghao11.cn

Java: u instanceof User
来源：http://jet.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cfh.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://xmy.chenlongwang.top

C#:   u is User
来源：http://tid.hysaishi.cn

[G14] 数据类 / record
来源：http://hmv.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zny.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://xxd.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://jan.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://ufu.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://kfb.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://tob.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ywz.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://ifa.jlsjyb.cn

[G15] 枚举
来源：http://okl.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eys.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mli.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hpm.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lad.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://qex.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cmx.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://spm.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://szt.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://pmo.hesvh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vcp.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://ewa.cqqwz.cn

JS:   Object.entries(obj)
来源：http://mru.zdbjq.cn

TS:   Object.entries(obj)
来源：http://jrh.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tyt.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://okr.svipenyu.cn

Ruby: obj.instance_variables
来源：http://llm.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://xgq.ydzc1.top

================================================================================
来源：http://zeo.yj202588.top

H. 异常与错误处理
来源：http://uww.hammf.cn

================================================================================
来源：http://pmu.fehbvm.com

[H01] try / catch 基础
来源：http://cmv.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ldv.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ilv.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://edx.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qvm.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gdr.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hws.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qaq.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dxx.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://qxg.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://qvr.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://vmz.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wwa.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tqs.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://twp.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yav.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ucv.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ynf.tanke756.top

[H03] 主动抛出异常
来源：http://krb.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://ene.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zhq.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://ndz.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://hka.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vuf.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://psx.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tei.shanyushiyangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://vhs.chenlongwang.top

[H04] 自定义异常类型
来源：http://pgs.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://fyu.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://fww.vehdjk.com

JS:   class MyError extends Error {}
来源：http://oqb.sweek.top

TS:   class MyError extends Error {}
来源：http://vkm.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://aug.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hua.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://yna.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://rwt.jyoumei.cn

[H05] 捕获特定类型
来源：http://oor.zdqjudy.top

Py:   except ValueError as e:
来源：http://qpl.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zhq.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://vce.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ssv.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://ctg.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://njq.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://gwe.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tqa.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://wlc.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://vwt.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://qxq.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://etx.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hag.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jfm.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mly.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://cdh.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://cly.hnxiangtu.top

[H07] 断言
来源：http://vli.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://kpk.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://swt.yvedp.cn

JS:   console.assert(x > 0);
来源：http://fyr.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://jvy.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://vok.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ecq.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://igl.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://jiv.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://vdf.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://usv.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wsg.yonumen.top

JS:   e.message;  e.stack
来源：http://cpu.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ivp.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ili.52xcode.cn

Go:   err.Error()
来源：http://cic.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://yka.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://xhk.ctjpmb.com

[H09] 带错误码的异常
来源：http://edl.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zrs.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jka.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aew.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ufh.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmg.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ecp.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://uql.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vml.cheryme.top

[H10] 资源自动释放
来源：http://onw.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tfo.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wdj.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ffm.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://guc.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fea.zycfv.cn

Go:   defer f.Close()
来源：http://cgq.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://akh.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yil.tianlin.xyz

================================================================================
来源：http://dhm.yueranfly.top

I. 正则表达式
来源：http://iit.hfpthk.cn

================================================================================
来源：http://upi.daxiang520.top

[I01] 判断是否匹配
来源：http://ldq.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jna.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xqy.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://ops.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://ttp.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dog.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hsz.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://gcj.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hnd.sweek.top

[I02] 提取所有匹配
来源：http://smb.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://zet.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hil.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://owo.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://jii.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://taz.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jti.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://plf.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pdo.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://tig.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jgj.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bgz.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ysl.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lkx.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wmf.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lqc.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tpa.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aus.smart0.xyz

[I04] 正则替换
来源：http://xxa.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sad.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dhp.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://www.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://qaf.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://pof.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jrm.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zny.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://scp.yongpay.top

[I05] 按正则拆分
来源：http://wvq.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://aqq.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uto.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://bdw.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://tce.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://fuh.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ahr.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rpo.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ctw.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bsi.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pqw.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lcd.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jht.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qto.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uii.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iff.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://met.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xwa.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://lui.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jws.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jpw.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://udb.wangshuangyany.cn

TS:   /error/gim
来源：http://kjd.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jzy.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cno.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://fvw.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ttg.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://mko.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nwg.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gvs.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eev.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqc.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://skb.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yjg.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qxu.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tti.tarul.cn

================================================================================
来源：http://lst.chenjidiqi.icu

J. 日期与时间
来源：http://wwf.yueranfly.top

================================================================================
来源：http://pmi.xinyue.icu

[J01] 获取当前时间
来源：http://yzs.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yzf.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gde.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://ekp.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://nze.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pos.jqgufenzy.top

Go:   time.Now()
来源：http://pqm.svipenyu.cn

Ruby: Time.now
来源：http://qcw.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kwc.sufxvd.cn

[J02] 格式化输出
来源：http://sqk.ivvv.top


<!-- 参考信息 -->