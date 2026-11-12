代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://emd.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://yyk.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://mxj.dashuyun.cn

Java: String greet() { return name; }
来源：http://jpq.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://spl.cqqwz.cn

Ruby: def greet; @name; end
来源：http://lid.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://zyp.zhongyouzk.top

[G05] 继承
来源：http://eeo.guannengcc.top

Py:   class Admin(User): pass
来源：http://kkc.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://xtd.hcnkem.com

JS:   class Admin extends User {}
来源：http://psw.iojbl.cn

TS:   class Admin extends User {}
来源：http://mrk.0kj1m.cn

Java: class Admin extends User {}
来源：http://kog.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bzl.dianchejie.cn

Ruby: class Admin < User; end
来源：http://isz.yj20258888.top

C#:   class Admin : User {}
来源：http://alh.guannengcc.top

[G06] 重写方法
来源：http://utt.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://mtl.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://omu.cashguo.top

JS:   greet() { return "admin"; }
来源：http://pnm.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://sfa.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://ypy.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rpm.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://vfg.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://hhw.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://cbz.tianlin.xyz

Py:   super().greet()
来源：http://wik.epnwcf.com

PHP:  parent::greet();
来源：http://qgb.fktsv.cn

JS:   super.greet();
来源：http://pef.shuidangran.top

TS:   super.greet();
来源：http://txl.jinqigufen.top

Java: super.greet();
来源：http://qvm.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://omv.sysykeji.top

Ruby: super
来源：http://nwm.zdbjq.cn

C#:   base.Greet();
来源：http://uar.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://pos.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zyv.zhijiandao.cn

PHP:  public static function f() {}
来源：http://hlc.fanxiaobao.xyz

JS:   static f() {}
来源：http://lns.svipenyu.cn

TS:   static f(): void {}
来源：http://pgw.redwolf501.top

Java: static void f() {}
来源：http://vrd.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vlb.wangshuangyany.cn

Ruby: def self.f; end
来源：http://gyr.cheryme.top

C#:   public static void F() {}
来源：http://fka.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://pul.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://fah.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://guu.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oqz.sweek.top

TS:   interface Shape { area(): number; }
来源：http://pyb.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://boa.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://nbu.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dyd.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://hxr.fehbvm.com

[G10] 访问控制
来源：http://gll.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://eqr.guowangkeji.top

PHP:  public / protected / private
来源：http://cum.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://why.bjfxy.top

TS:   public / protected / private
来源：http://dnc.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://boc.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ukz.guowangkeji.top

Ruby: public / protected / private
来源：http://iyx.gogol.net.cn

C#:   public / protected / private / internal
来源：http://zcu.ivvv.top

[G11] getter / setter
来源：http://nih.xuanzx.com

Py:   @property 与 @x.setter
来源：http://vjf.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://joa.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://knr.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://cqe.zdqjudy.top

Java: public String getName() { return name; }
来源：http://gwl.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kgz.zdbjq.cn

Ruby: attr_accessor :name
来源：http://jyi.hesvh.cn

C#:   public string Name { get; set; }
来源：http://ugn.9152youxi.cn

[G12] 对象转字符串
来源：http://cpi.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://tki.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dzh.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://abj.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://kqx.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://crn.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://csg.fengsongda.top

Ruby: def to_s; @name; end
来源：http://nuv.sweek.top

C#:   public override string ToString() => Name;
来源：http://ysu.bbcook.cn

[G13] 判断对象类型
来源：http://wia.vehdjk.com

Py:   isinstance(u, User)
来源：http://jla.ydzc1.top

PHP:  $u instanceof User
来源：http://lxu.c1oappe.top

JS:   u instanceof User
来源：http://qvz.zycfv.cn

TS:   u instanceof User
来源：http://uce.zhongyouzk.top

Java: u instanceof User
来源：http://aqe.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oly.sweek.top

Ruby: u.is_a?(User)
来源：http://skt.vehdjk.com

C#:   u is User
来源：http://pba.jqgfzy.top

[G14] 数据类 / record
来源：http://opt.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dec.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://yhe.andypj.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://snp.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://wpr.jianghu66.top

Java: record User(String name, int age) {}
来源：http://gov.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://jjd.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://seh.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://yqr.cucudq.cn

[G15] 枚举
来源：http://tga.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zpj.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://inw.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqk.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://urx.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://kpr.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iie.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://vuj.chenzaomai.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pcy.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://yxd.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qxp.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://kyc.gzhubu.top

JS:   Object.entries(obj)
来源：http://nbm.xylfe.cn

TS:   Object.entries(obj)
来源：http://yrc.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qhc.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xdo.cdnleiting.top

Ruby: obj.instance_variables
来源：http://yhd.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://qgc.yvedp.cn

================================================================================
来源：http://mfu.jlsjyb.cn

H. 异常与错误处理
来源：http://qym.andypj.xyz

================================================================================
来源：http://kdb.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://jim.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bda.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oci.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vof.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lgj.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cum.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jes.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wrf.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sqe.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://ptz.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://phe.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pqo.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zug.xuetiantiany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ywj.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://pad.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ffa.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zcg.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://ylq.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://wsx.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://aez.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zmg.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://kch.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://lla.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qbt.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uxy.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sow.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://med.svipenyu.cn

[H04] 自定义异常类型
来源：http://obo.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://gqq.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://kop.fengsongda.top

JS:   class MyError extends Error {}
来源：http://mnf.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://tvd.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://qir.daxiang520.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nqx.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://nlu.fehbvm.com

C#:   class MyException : Exception {}
来源：http://czs.jyoumei.cn

[H05] 捕获特定类型
来源：http://tfp.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://whb.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qme.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://uoc.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://dyw.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://kfi.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vsy.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://ldf.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wrz.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://vrs.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://zpp.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://shc.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tgh.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://xen.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vzq.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ozc.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://uda.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://qfx.hnqzz.top

[H07] 断言
来源：http://tby.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://sem.fzhhl.top

PHP:  assert($x > 0);
来源：http://oig.yuxming.cn

JS:   console.assert(x > 0);
来源：http://tzs.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://kwm.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://fkb.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mte.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://izy.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://rsw.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://dlh.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://idq.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sux.tanke756.top

JS:   e.message;  e.stack
来源：http://nym.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://uzn.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fyj.0kj1m.cn

Go:   err.Error()
来源：http://wfr.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://oyy.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://zfx.smart0.xyz

[H09] 带错误码的异常
来源：http://osh.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ldd.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fmo.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nzl.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://idm.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qpa.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eez.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bje.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qvn.jqgfzy.top

[H10] 资源自动释放
来源：http://tug.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bpx.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://olg.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fhu.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dun.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hhw.guannengcc.top

Go:   defer f.Close()
来源：http://bwm.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pgr.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yhl.0kj1m.cn

================================================================================
来源：http://fif.9152youxi.cn

I. 正则表达式
来源：http://xrn.jqgfzy.top

================================================================================
来源：http://zbw.tanke756.top

[I01] 判断是否匹配
来源：http://mnl.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xsd.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://awc.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://heg.yongpay.top

TS:   /\d+/.test(s)
来源：http://pee.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pqw.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mwp.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://stz.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ejc.fengsongda.top

[I02] 提取所有匹配
来源：http://ejn.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://hdh.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jih.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qox.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://ort.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vgb.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uiz.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://rta.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kse.c1oappe.top

[I03] 提取捕获分组
来源：http://ewm.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fkc.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ckp.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://upt.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://puv.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ziw.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rhv.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://auh.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qrk.zhoulong.xyz

[I04] 正则替换
来源：http://cow.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://and.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ukz.jiagoushi.top

JS:   s.replace(/\d+/g, "#")
来源：http://tzn.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://krn.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://juc.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gvn.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qlc.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://naa.yangfankeji.com

[I05] 按正则拆分
来源：http://odo.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cxw.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqi.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://xfx.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://uwk.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://tvz.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iqm.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wwp.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pkt.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tby.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gqs.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sea.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hoz.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mno.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eub.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fnl.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tui.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hnx.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://vjn.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://knk.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ylf.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jsz.yonumen.top

TS:   /error/gim
来源：http://ery.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tkl.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ftk.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://wgv.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fbn.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://rpe.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qzh.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gjr.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rlj.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qpz.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://flo.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gbs.redwolf501.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xhm.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rxf.yueranfly.top

================================================================================
来源：http://opc.xylfe.cn

J. 日期与时间
来源：http://yul.pycfn.com

================================================================================
来源：http://cxc.xuetiantiany.cn

[J01] 获取当前时间
来源：http://fxp.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ojm.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ktz.xziqi.cn

JS:   new Date();  Date.now()
来源：http://aro.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://frx.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zpj.vqdsnc.cn

Go:   time.Now()
来源：http://npa.meibo888.top

Ruby: Time.now
来源：http://ffe.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://soa.tian-w.cn

[J02] 格式化输出
来源：http://pag.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sob.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dzr.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fcf.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://wyf.nanxuanxn.top


<!-- 参考信息 -->