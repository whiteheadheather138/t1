代发 wailian999

TS:   constructor(public name: string) {}
来源：http://osw.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://enu.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aju.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://nha.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://cui.quarkkingdee.top

[G03] 实例属性
来源：http://tox.yuxming.cn

Py:   self.name = "x"
来源：http://ict.yj202588.top

PHP:  public string $name = "x";
来源：http://kye.svipenyu.cn

JS:   this.name = "x";
来源：http://wca.yj202588.top

TS:   name: string = "x";
来源：http://pzi.ivvv.top

Java: private String name;
来源：http://zif.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qcg.sweek.top

Ruby: @name = "x"
来源：http://dmd.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://veo.aibaodan.cn

[G04] 定义方法
来源：http://rgp.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://yje.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gmx.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://kud.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://qxu.ehwqpu.com

Java: String greet() { return name; }
来源：http://pfj.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://zai.hesvh.cn

Ruby: def greet; @name; end
来源：http://gdq.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://ufi.uphjek.com

[G05] 继承
来源：http://ayd.zdbjq.cn

Py:   class Admin(User): pass
来源：http://twy.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://oux.hcnkem.com

JS:   class Admin extends User {}
来源：http://bcq.cashguo.top

TS:   class Admin extends User {}
来源：http://dqt.xinyue.icu

Java: class Admin extends User {}
来源：http://vxa.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iih.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://agn.jiagoushi.top

C#:   class Admin : User {}
来源：http://vzh.xinyue.icu

[G06] 重写方法
来源：http://ftx.yongpay.top

Py:   def greet(self): return "admin"
来源：http://kxn.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://sqd.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://dcm.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://ldb.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://rad.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rkn.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://lnl.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://uou.tianlin.xyz

[G07] 调用父类方法
来源：http://aox.hywenlv.cn

Py:   super().greet()
来源：http://caa.iojbl.cn

PHP:  parent::greet();
来源：http://axi.daria6918.cn

JS:   super.greet();
来源：http://epi.316326.xyz

TS:   super.greet();
来源：http://idk.hcnkem.com

Java: super.greet();
来源：http://jsh.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nls.zhijiandao.cn

Ruby: super
来源：http://tgc.shuidangran.top

C#:   base.Greet();
来源：http://pji.hcnkem.com

[G08] 静态方法与属性
来源：http://uzd.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ngk.jinqigfzy.top

PHP:  public static function f() {}
来源：http://hhe.feifeiyinyue.top

JS:   static f() {}
来源：http://yhw.52xcode.cn

TS:   static f(): void {}
来源：http://oiv.gzhubu.top

Java: static void f() {}
来源：http://mqt.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lan.chenjidiqi.icu

Ruby: def self.f; end
来源：http://fra.daxiang520.top

C#:   public static void F() {}
来源：http://rul.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://ewn.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://atg.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tez.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lfd.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://exz.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://nqz.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://tsb.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jzj.xinyue.icu

C#:   interface IShape { double Area(); }
来源：http://rth.bbcook.cn

[G10] 访问控制
来源：http://jkr.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://hwl.fzhhl.top

PHP:  public / protected / private
来源：http://urs.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://ocp.zhijiandao.cn

TS:   public / protected / private
来源：http://emp.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://ldi.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bkg.pengpengdd.cyou

Ruby: public / protected / private
来源：http://rlb.ppjwa.cn

C#:   public / protected / private / internal
来源：http://xtf.redwolf501.top

[G11] getter / setter
来源：http://fnr.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://rvh.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sks.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://eeo.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://qtv.aibaodan.cn

Java: public String getName() { return name; }
来源：http://jvr.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://edl.wangdashe.top

Ruby: attr_accessor :name
来源：http://kty.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://olb.haohaochexian.top

[G12] 对象转字符串
来源：http://szh.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://mnn.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://fqv.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://twh.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://one.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://zzw.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fhp.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://tno.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://xlq.zhengqikj.top

[G13] 判断对象类型
来源：http://xgw.havefunace.top

Py:   isinstance(u, User)
来源：http://nwb.cucudq.cn

PHP:  $u instanceof User
来源：http://cfu.guannengcc.top

JS:   u instanceof User
来源：http://sul.daria6918.cn

TS:   u instanceof User
来源：http://juq.shzxlz.cn

Java: u instanceof User
来源：http://ynd.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uvn.316326.xyz

Ruby: u.is_a?(User)
来源：http://kkv.jqgfzy.top

C#:   u is User
来源：http://xud.ctjpmb.com

[G14] 数据类 / record
来源：http://jcx.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cnj.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jlw.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://zsz.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://ofc.epnwcf.com

Java: record User(String name, int age) {}
来源：http://str.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://pgo.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gub.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://jlo.zycfv.cn

[G15] 枚举
来源：http://dfr.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oft.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ihg.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pta.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zyj.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://gul.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://loh.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://uff.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://acw.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://fut.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vez.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://ilf.tanke756.top

JS:   Object.entries(obj)
来源：http://trj.cheryme.top

TS:   Object.entries(obj)
来源：http://hue.chenzaomai.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://svk.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://lej.dianchejie.cn

Ruby: obj.instance_variables
来源：http://jci.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://tfz.pengpengdd.cyou

================================================================================
来源：http://wpl.ybcxt.top

H. 异常与错误处理
来源：http://bub.yuanzhike.top

================================================================================
来源：http://yun.gzhubu.top

[H01] try / catch 基础
来源：http://wkz.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tsc.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tej.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nhn.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xkg.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://geb.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rqu.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dnb.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pvf.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://til.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ajf.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lod.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qxx.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://uzm.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://xpc.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://skw.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oud.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ilq.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://jqe.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://xyw.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vut.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://xtl.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://bmu.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cdr.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aqp.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://svc.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hwj.jlsjyb.cn

[H04] 自定义异常类型
来源：http://ono.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://vlo.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pei.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://gnj.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://rvn.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://ysf.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nha.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://ebx.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://hka.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://pet.mhx1999.top

Py:   except ValueError as e:
来源：http://ibk.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bdp.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://tnl.jinghuilouyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://inu.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://zqm.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hhq.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://jjr.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sji.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://dba.yuxming.cn

Py:   value = d.get("k") or default
来源：http://jcu.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://ofq.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vkz.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ejs.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sfr.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://feu.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://aub.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://beo.fanxiaobao.xyz

[H07] 断言
来源：http://kzz.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://idm.uphjek.com

PHP:  assert($x > 0);
来源：http://yof.xziqi.cn

JS:   console.assert(x > 0);
来源：http://sch.c1oappe.top

TS:   console.assert(x > 0);
来源：http://evb.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://udm.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://osr.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fzx.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://gwb.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://vqs.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://fgp.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ugd.cqqwz.cn

JS:   e.message;  e.stack
来源：http://tob.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bmu.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tzf.ydjk.org.cn

Go:   err.Error()
来源：http://gbf.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://aoc.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://rpi.cdnleiting.top

[H09] 带错误码的异常
来源：http://kjx.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iwx.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjr.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tvf.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wjz.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fpk.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxv.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://chk.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://msx.zhijiandao.cn

[H10] 资源自动释放
来源：http://tip.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tdl.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fha.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iez.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bes.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qlw.yuxming.cn

Go:   defer f.Close()
来源：http://xua.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://suc.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hhc.vqdsnc.cn

================================================================================
来源：http://fcz.yj20258.top

I. 正则表达式
来源：http://rju.zdbjq.cn

================================================================================
来源：http://wen.hcnkem.com

[I01] 判断是否匹配
来源：http://voa.hywenlv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xzz.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://cpy.ydzc1.top

JS:   /\d+/.test(s)
来源：http://zaa.cheryme.top

TS:   /\d+/.test(s)
来源：http://nao.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://odh.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uwj.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://blc.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zex.uphjek.com

[I02] 提取所有匹配
来源：http://fua.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://ule.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eue.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qjg.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://iwb.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hxb.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sqa.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://jgv.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gnc.quarkkingdee.top

[I03] 提取捕获分组
来源：http://eky.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ejc.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ogq.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bif.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fzx.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yqb.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rfw.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sce.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kia.shangyingyoupin.top

[I04] 正则替换
来源：http://vkr.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wci.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jxc.jiagoushi.top

JS:   s.replace(/\d+/g, "#")
来源：http://jna.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ujg.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://dqk.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://veh.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://noq.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tyx.yanxiufei.cn

[I05] 按正则拆分
来源：http://vsa.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://arw.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baj.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://eul.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://fsm.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://tcz.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yjs.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://gkn.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cin.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ssg.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://alm.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iwj.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://doi.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://umv.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzr.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bmk.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gxj.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nqu.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://edo.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fdu.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tte.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lyu.cdnleiting.top

TS:   /error/gim
来源：http://dfq.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gyr.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hzi.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://fqp.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zbo.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://ajy.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://has.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jfh.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjk.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://grz.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qnd.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dmo.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ver.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iib.fengsongda.top

================================================================================
来源：http://bnp.ydjk.org.cn


<!-- 参考信息 -->