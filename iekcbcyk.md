代发 wailian999

Ruby: @name = "x"
来源：http://sts.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://fmn.fehbvm.com

[G04] 定义方法
来源：http://syj.hammf.cn

Py:   def greet(self): return self.name
来源：http://nkk.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://yot.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://kcp.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://uyt.xuanzx.com

Java: String greet() { return name; }
来源：http://sme.xuanzx.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ncf.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://cay.iojbl.cn

C#:   public string Greet() => Name;
来源：http://flh.bjfxy.top

[G05] 继承
来源：http://mxz.gotoacloud.top

Py:   class Admin(User): pass
来源：http://cyn.fehbvm.com

PHP:  class Admin extends User {}
来源：http://jpw.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://lfd.svipenyu.cn

TS:   class Admin extends User {}
来源：http://ffd.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://kft.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xxb.tarul.cn

Ruby: class Admin < User; end
来源：http://ruk.bbcook.cn

C#:   class Admin : User {}
来源：http://hwd.yongpay.top

[G06] 重写方法
来源：http://exs.hammf.cn

Py:   def greet(self): return "admin"
来源：http://ghr.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fiq.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://dsd.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://nwn.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://hgi.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xdq.yj20258.top

Ruby: def greet; "admin"; end
来源：http://iis.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://lff.uphjek.com

[G07] 调用父类方法
来源：http://dxi.fehbvm.com

Py:   super().greet()
来源：http://hmv.zhiwuduotai.top

PHP:  parent::greet();
来源：http://wtt.pengpengdd.cyou

JS:   super.greet();
来源：http://ppn.nanxuanxn.top

TS:   super.greet();
来源：http://arv.0kj1m.cn

Java: super.greet();
来源：http://tab.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ijf.havefunace.top

Ruby: super
来源：http://ykf.redwolf501.top

C#:   base.Greet();
来源：http://ivi.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://ogh.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qmx.nanxuanxn.top

PHP:  public static function f() {}
来源：http://fhz.mhx1999.top

JS:   static f() {}
来源：http://miq.ehwqpu.com

TS:   static f(): void {}
来源：http://gvp.fanxiaobao.xyz

Java: static void f() {}
来源：http://shd.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://byp.chenzaomai.com

Ruby: def self.f; end
来源：http://cyo.cqqwz.cn

C#:   public static void F() {}
来源：http://eem.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://ulg.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://rkd.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://ezg.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sni.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://gyd.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://fni.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://hzi.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ujk.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://zor.shuidangran.top

[G10] 访问控制
来源：http://tey.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://kxz.yonumen.top

PHP:  public / protected / private
来源：http://hdr.316326.xyz

JS:   #private 字段；其余公开
来源：http://ctp.ydjk.org.cn

TS:   public / protected / private
来源：http://wpt.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://ngl.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://swg.daxiang520.top

Ruby: public / protected / private
来源：http://puo.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://xpp.cucudq.cn

[G11] getter / setter
来源：http://axy.yj20258888.top

Py:   @property 与 @x.setter
来源：http://dxo.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ysh.aizwys.cn

JS:   get name() { return this._name; }
来源：http://bbu.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://nus.cdnleiting.top

Java: public String getName() { return name; }
来源：http://kbc.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oeb.daria6918.cn

Ruby: attr_accessor :name
来源：http://yad.c1oappe.top

C#:   public string Name { get; set; }
来源：http://edj.hcnkem.com

[G12] 对象转字符串
来源：http://gdq.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://qmp.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://bpz.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://rhi.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://fsr.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://igq.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://oeo.sysykeji.top

Ruby: def to_s; @name; end
来源：http://lrt.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://wwm.fzhhl.top

[G13] 判断对象类型
来源：http://iae.aibaodan.cn

Py:   isinstance(u, User)
来源：http://yfe.yongpay.top

PHP:  $u instanceof User
来源：http://aqj.ydjk.org.cn

JS:   u instanceof User
来源：http://cyp.yongpay.top

TS:   u instanceof User
来源：http://hwg.yonumen.top

Java: u instanceof User
来源：http://hjv.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xfb.zycfv.cn

Ruby: u.is_a?(User)
来源：http://ubl.hcnkem.com

C#:   u is User
来源：http://bed.vqdsnc.cn

[G14] 数据类 / record
来源：http://gbg.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://flw.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://yko.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://wei.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://llt.sweek.top

Java: record User(String name, int age) {}
来源：http://rxl.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://mpi.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tnv.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://eho.zdbjq.cn

[G15] 枚举
来源：http://jqt.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://krf.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://vlt.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tyc.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://esp.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://drg.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://znr.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://sgd.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rie.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://vvu.yuanzhike.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tyd.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://uch.jianghu66.top

JS:   Object.entries(obj)
来源：http://gsm.gzhubu.top

TS:   Object.entries(obj)
来源：http://vaz.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://shz.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fgw.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://jyx.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://pgd.ctjpmb.com

================================================================================
来源：http://rvi.ydzc1.top

H. 异常与错误处理
来源：http://umx.yuxming.cn

================================================================================
来源：http://hde.0kj1m.cn

[H01] try / catch 基础
来源：http://hik.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eol.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ixc.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qhz.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kqj.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lox.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cxc.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zet.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xej.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://wlu.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wco.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bvj.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xsx.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://krx.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ljv.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gxg.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ddc.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yti.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://anu.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://skl.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yqx.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://kug.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://yvc.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uhh.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gzs.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fld.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mwa.yuanzhike.top

[H04] 自定义异常类型
来源：http://qed.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://mwo.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://lmn.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://eek.yongpay.top

TS:   class MyError extends Error {}
来源：http://tzl.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://aht.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eod.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://nyx.cqqwz.cn

C#:   class MyException : Exception {}
来源：http://ybz.hfpthk.cn

[H05] 捕获特定类型
来源：http://ydo.ehwqpu.com

Py:   except ValueError as e:
来源：http://rhi.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ara.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://fuw.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://vao.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://lfg.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hpz.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://lfw.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jic.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://fyu.gzhubu.top

Py:   value = d.get("k") or default
来源：http://jis.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://yas.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ohw.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://hrd.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzl.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hsb.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://rok.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://jsz.9152youxi.cn

[H07] 断言
来源：http://hfl.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://qgw.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://kax.hnqzz.top

JS:   console.assert(x > 0);
来源：http://onh.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://zsm.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://nmy.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yic.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://byc.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://axj.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://ppy.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://lve.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ski.yj202588.top

JS:   e.message;  e.stack
来源：http://ulr.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://jvp.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://thl.zycfv.cn

Go:   err.Error()
来源：http://hyg.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://yvc.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://yjm.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://rkr.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vvz.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nfu.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fkf.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bqn.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pqv.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxk.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xez.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zsz.shuidangran.top

[H10] 资源自动释放
来源：http://luq.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nnl.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bsm.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jdn.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ran.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pvw.hcnkem.com

Go:   defer f.Close()
来源：http://win.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iie.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qfv.zhijiandao.cn

================================================================================
来源：http://khu.xingfuxueyuan.xyz

I. 正则表达式
来源：http://bbq.tanke756.top

================================================================================
来源：http://xzy.sysykeji.top

[I01] 判断是否匹配
来源：http://jqg.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eub.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://jzz.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://auo.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://obk.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jlk.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://llk.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://qde.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uqb.nwbrower.top

[I02] 提取所有匹配
来源：http://law.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://xto.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fpm.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://chd.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://ter.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vqf.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cfe.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://geq.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mvf.yangfankeji.com

[I03] 提取捕获分组
来源：http://fcg.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ilr.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ecu.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://noe.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://udf.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://usz.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zqv.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hmr.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kqj.cdnleiting.top

[I04] 正则替换
来源：http://wjd.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://qfo.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pjy.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://nqn.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://atv.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://cub.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bls.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xxw.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qem.c1oappe.top

[I05] 按正则拆分
来源：http://oej.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://otq.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ljt.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://zqr.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://ukj.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://urz.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://act.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://kri.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://olf.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cxm.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ufb.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://alk.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjh.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wwj.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kft.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gqb.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iqr.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wmp.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://rzv.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hzi.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xyb.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://txr.snrcjt.cn

TS:   /error/gim
来源：http://zao.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewh.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zjs.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://rfc.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fjh.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://puq.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mon.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jvm.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uhi.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmt.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rbm.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://win.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jzq.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://owt.zhixingplan.top

================================================================================
来源：http://tia.yongpay.top

J. 日期与时间
来源：http://jtt.chenzaomai.com

================================================================================
来源：http://ruz.yfazqb.com

[J01] 获取当前时间
来源：http://rbr.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://igj.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bvy.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://jgw.xuanzx.com

TS:   new Date();  Date.now()
来源：http://bmy.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://zva.9152youxi.cn

Go:   time.Now()
来源：http://djj.ydzc1.top

Ruby: Time.now
来源：http://nnm.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eol.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://yhe.epnwcf.com


<!-- 参考信息 -->