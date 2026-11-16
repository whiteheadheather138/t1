代发 wailian999

TS:   constructor(public name: string) {}
来源：http://rye.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://brk.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hlr.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://szu.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://huk.yj202588.top

[G03] 实例属性
来源：http://zgd.zycfv.cn

Py:   self.name = "x"
来源：http://qtw.iojbl.cn

PHP:  public string $name = "x";
来源：http://ylg.bbcook.cn

JS:   this.name = "x";
来源：http://qcc.ctjpmb.com

TS:   name: string = "x";
来源：http://muy.zhaomingkeji.xyz

Java: private String name;
来源：http://ahr.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://miy.jqgufenzy.top

Ruby: @name = "x"
来源：http://xld.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://qdd.jiagoushi.top

[G04] 定义方法
来源：http://ide.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://igd.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zsd.tarul.cn

JS:   greet() { return this.name; }
来源：http://qgn.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://hkg.tian-w.cn

Java: String greet() { return name; }
来源：http://obq.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kow.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://evr.sweek.top

C#:   public string Greet() => Name;
来源：http://wnk.9152youxi.cn

[G05] 继承
来源：http://aqq.daxiang520.top

Py:   class Admin(User): pass
来源：http://ckh.epnwcf.com

PHP:  class Admin extends User {}
来源：http://tnj.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://djr.vehdjk.com

TS:   class Admin extends User {}
来源：http://dvk.hywenlv.cn

Java: class Admin extends User {}
来源：http://znw.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wbq.jianghu66.top

Ruby: class Admin < User; end
来源：http://iyf.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://eux.quarkkingdee.top

[G06] 重写方法
来源：http://joc.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://ofi.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zsc.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://jap.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://mwn.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://xcd.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bbb.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://ijz.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://vhx.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://kph.yj20258888.top

Py:   super().greet()
来源：http://eew.jqgfzy.top

PHP:  parent::greet();
来源：http://clf.cdnleiting.top

JS:   super.greet();
来源：http://tox.52xcode.cn

TS:   super.greet();
来源：http://mih.yuxming.cn

Java: super.greet();
来源：http://gxw.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xpi.hnxiangtu.top

Ruby: super
来源：http://uca.shuidangran.top

C#:   base.Greet();
来源：http://nrk.tarul.cn

[G08] 静态方法与属性
来源：http://qro.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kjh.iojbl.cn

PHP:  public static function f() {}
来源：http://nbv.fengsongda.top

JS:   static f() {}
来源：http://ktl.zhoulong.xyz

TS:   static f(): void {}
来源：http://dmj.sufxvd.cn

Java: static void f() {}
来源：http://yzp.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yca.chenzaomai.com

Ruby: def self.f; end
来源：http://zws.hnqzz.top

C#:   public static void F() {}
来源：http://fcc.hnqzz.top

[G09] 接口 / 抽象类
来源：http://yya.ydjk.org.cn

Py:   from abc import ABC, abstractmethod
来源：http://zpw.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://toc.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqb.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://uqf.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://hji.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://pip.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gyf.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://uio.vqdsnc.cn

[G10] 访问控制
来源：http://esi.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://rjd.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://tth.snrcjt.cn

JS:   #private 字段；其余公开
来源：http://abl.aibaodan.cn

TS:   public / protected / private
来源：http://isp.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://vbr.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qlv.epnwcf.com

Ruby: public / protected / private
来源：http://ick.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://jve.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://aqd.iojbl.cn

Py:   @property 与 @x.setter
来源：http://soc.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fcs.vehdjk.com

JS:   get name() { return this._name; }
来源：http://vsf.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://ord.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://rho.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ioj.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://blz.c1oappe.top

C#:   public string Name { get; set; }
来源：http://fek.cheryme.top

[G12] 对象转字符串
来源：http://azm.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://gth.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://wlx.yj20258888.top

JS:   toString() { return this.name; }
来源：http://qsn.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://iqx.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ixz.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://idc.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://cjj.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://vaz.hfpthk.cn

[G13] 判断对象类型
来源：http://wbr.snrcjt.cn

Py:   isinstance(u, User)
来源：http://cbm.zdbjq.cn

PHP:  $u instanceof User
来源：http://cmi.shuidangran.top

JS:   u instanceof User
来源：http://jur.gzhubu.top

TS:   u instanceof User
来源：http://izx.0kj1m.cn

Java: u instanceof User
来源：http://ugm.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sci.shuidangran.top

Ruby: u.is_a?(User)
来源：http://gfu.iojbl.cn

C#:   u is User
来源：http://rne.gaohongyu789.top

[G14] 数据类 / record
来源：http://xqs.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ysy.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://mrf.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hgn.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://zqd.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://niw.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://ipx.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bzp.birdmap.top

C#:   record User(string Name, int Age);
来源：http://fuu.shzxlz.cn

[G15] 枚举
来源：http://iuj.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://naw.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsm.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wwv.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ryb.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://xof.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ktf.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://huf.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aji.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://jut.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yvd.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://azo.zhixingplan.top

JS:   Object.entries(obj)
来源：http://idy.yj202588.top

TS:   Object.entries(obj)
来源：http://mhj.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rps.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cup.jinqigufen.top

Ruby: obj.instance_variables
来源：http://ewd.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://vjo.sufxvd.cn

================================================================================
来源：http://ssq.fzhhl.top

H. 异常与错误处理
来源：http://cav.nanxuanxn.top

================================================================================
来源：http://bvr.wangshuangyany.cn

[H01] try / catch 基础
来源：http://xws.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qvr.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fhs.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iya.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iso.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eds.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ekt.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bvu.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://keg.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://mpc.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xiv.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://knr.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zrk.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://luk.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://utu.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://pic.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fyj.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://clj.jianghu66.top

[H03] 主动抛出异常
来源：http://cwp.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://ylx.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wbw.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://dyf.316326.xyz

TS:   throw new Error("错误信息");
来源：http://gmj.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ytb.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://idh.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://snp.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://yrg.fktsv.cn

[H04] 自定义异常类型
来源：http://xrw.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://mhp.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://uwf.yonumen.top

JS:   class MyError extends Error {}
来源：http://jmr.nwbrower.top

TS:   class MyError extends Error {}
来源：http://vnq.ydzc1.top

Java: class MyException extends RuntimeException {}
来源：http://zha.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybc.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://vwd.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://gaa.zhengqikj.top

[H05] 捕获特定类型
来源：http://kqj.yanxiufei.cn

Py:   except ValueError as e:
来源：http://yau.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mik.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://zpm.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://yhl.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://xgz.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qdg.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://bjw.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pak.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://gak.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://bko.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://iix.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://you.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://ryt.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xpy.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uwo.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://dzv.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://ifc.fengsongda.top

[H07] 断言
来源：http://eyy.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://gbs.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://bde.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://rux.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://wgv.bbcook.cn

Java: assert x > 0 : "必须为正";
来源：http://fcy.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lng.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://csl.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://puu.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://afl.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://lpm.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://she.ppjwa.cn

JS:   e.message;  e.stack
来源：http://tkf.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://azx.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xhx.tanke756.top

Go:   err.Error()
来源：http://hha.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://gkp.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://epc.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://tfx.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dqa.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bzv.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dps.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yuh.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fks.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xpo.zycfv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ubh.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ues.meibo888.top

[H10] 资源自动释放
来源：http://lxx.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pws.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qhc.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jfc.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sab.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gtg.c1oappe.top

Go:   defer f.Close()
来源：http://lnk.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fsi.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iiw.cheryme.top

================================================================================
来源：http://pxv.jinqigfzy.top

I. 正则表达式
来源：http://inq.yj202588.top

================================================================================
来源：http://vsm.tarul.cn

[I01] 判断是否匹配
来源：http://sao.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ive.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://ujo.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://bvg.sxryk.cn

TS:   /\d+/.test(s)
来源：http://mwj.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gjy.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ejm.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://rbl.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xkm.sjlbkw.cn

[I02] 提取所有匹配
来源：http://kdf.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://uhs.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://suk.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jvd.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://eau.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hoi.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mjv.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://mjm.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nhs.yongpay.top

[I03] 提取捕获分组
来源：http://tvw.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vjk.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ktj.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wui.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://guv.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hxp.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ocr.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ain.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oxb.pycfn.com

[I04] 正则替换
来源：http://noe.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jze.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rsw.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://plh.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://lhc.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://drs.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yvz.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hog.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://soq.mhx1999.top

[I05] 按正则拆分
来源：http://kxh.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://srt.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ijz.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://idc.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://itc.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://fvy.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ove.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://sfk.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uvw.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uek.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tog.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lhv.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hwo.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvj.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://igm.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://suv.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://svf.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdd.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://sqn.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dfu.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jdl.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://scf.ivvv.top

TS:   /error/gim
来源：http://dhy.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oeb.zhaomingkeji.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zen.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://lct.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://niu.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://pdc.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xcw.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://skb.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://axu.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yhs.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tgr.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jop.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cfe.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://peq.daxiang520.top

================================================================================
来源：http://kxg.shzxlz.cn


<!-- 参考信息 -->