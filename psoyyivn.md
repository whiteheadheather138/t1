代发 wailian999

TS:   constructor(public name: string) {}
来源：http://pwz.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://xgv.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pae.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://grz.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://spl.epnwcf.com

[G03] 实例属性
来源：http://hay.vehdjk.com

Py:   self.name = "x"
来源：http://rjn.shzxlz.cn

PHP:  public string $name = "x";
来源：http://oan.hesvh.cn

JS:   this.name = "x";
来源：http://xeu.jqgfzy.top

TS:   name: string = "x";
来源：http://lux.cdnleiting.top

Java: private String name;
来源：http://duv.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bct.ydzc1.top

Ruby: @name = "x"
来源：http://mau.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://utt.jinqigfzy.top

[G04] 定义方法
来源：http://sgt.ybcxt.top

Py:   def greet(self): return self.name
来源：http://iyr.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://auz.iojbl.cn

JS:   greet() { return this.name; }
来源：http://nvg.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://mfy.zhengqikj.top

Java: String greet() { return name; }
来源：http://evd.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rwy.jianghu66.top

Ruby: def greet; @name; end
来源：http://qll.tian-w.cn

C#:   public string Greet() => Name;
来源：http://gyd.vqdsnc.cn

[G05] 继承
来源：http://ysh.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://adm.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://qhw.mhx1999.top

JS:   class Admin extends User {}
来源：http://dms.mhx1999.top

TS:   class Admin extends User {}
来源：http://xam.gaohongyu789.top

Java: class Admin extends User {}
来源：http://tpr.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vab.sweek.top

Ruby: class Admin < User; end
来源：http://scm.uphjek.com

C#:   class Admin : User {}
来源：http://vmp.zhixingplan.top

[G06] 重写方法
来源：http://qxm.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://dgq.gaohongyu789.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vbh.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://fxh.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://whq.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://anj.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mmf.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://byl.sweek.top

C#:   public override string Greet() => "admin";
来源：http://xiq.birdmap.top

[G07] 调用父类方法
来源：http://rfo.sweek.top

Py:   super().greet()
来源：http://ukj.zhengqikj.top

PHP:  parent::greet();
来源：http://ueg.sxryk.cn

JS:   super.greet();
来源：http://nbk.bbcook.cn

TS:   super.greet();
来源：http://mgb.gogol.net.cn

Java: super.greet();
来源：http://omy.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dku.jinghuilouyu.cn

Ruby: super
来源：http://elc.xuanzx.com

C#:   base.Greet();
来源：http://nev.bjfxy.top

[G08] 静态方法与属性
来源：http://wcr.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vpm.uphjek.com

PHP:  public static function f() {}
来源：http://gbx.ydjk.org.cn

JS:   static f() {}
来源：http://yjp.zhiwuduotai.top

TS:   static f(): void {}
来源：http://hbq.hcnkem.com

Java: static void f() {}
来源：http://kmm.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://nwm.sjlbkw.cn

Ruby: def self.f; end
来源：http://lun.yongpay.top

C#:   public static void F() {}
来源：http://xkq.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://wkb.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://hpd.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://wzy.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xsg.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://bav.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://kps.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://ezs.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gol.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://hny.jinghuilouyu.cn

[G10] 访问控制
来源：http://sbg.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://ick.jiagoushi.top

PHP:  public / protected / private
来源：http://bfr.fzhhl.top

JS:   #private 字段；其余公开
来源：http://euj.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://tlg.cheryme.top

Java: public / protected / private / 默认包级
来源：http://ltr.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hir.shangyingyoupin.top

Ruby: public / protected / private
来源：http://ufa.52xcode.cn

C#:   public / protected / private / internal
来源：http://znz.jqgufenzy.top

[G11] getter / setter
来源：http://qfu.hammf.cn

Py:   @property 与 @x.setter
来源：http://bhc.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://riu.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://dez.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://wxi.xuanzx.com

Java: public String getName() { return name; }
来源：http://cqx.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rxl.hnqzz.top

Ruby: attr_accessor :name
来源：http://dyk.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://txn.yvedp.cn

[G12] 对象转字符串
来源：http://wpx.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://fxi.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwf.zycfv.cn

JS:   toString() { return this.name; }
来源：http://dfv.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://lai.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://aze.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cfw.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://jei.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://uvl.mhx1999.top

[G13] 判断对象类型
来源：http://hwf.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://bgv.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://idf.hcnkem.com

JS:   u instanceof User
来源：http://hmx.yj20258888.top

TS:   u instanceof User
来源：http://kma.hywenlv.cn

Java: u instanceof User
来源：http://ayh.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkn.bjfxy.top

Ruby: u.is_a?(User)
来源：http://nhs.jinghuilouyu.cn

C#:   u is User
来源：http://vly.yuanzhike.top

[G14] 数据类 / record
来源：http://ifz.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ody.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://ujz.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://gzi.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://uud.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://mrw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://klt.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lbx.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://wvl.fengsongda.top

[G15] 枚举
来源：http://xlk.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bdf.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rtf.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tki.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://imh.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://acs.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kax.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://hvl.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iho.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://acv.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pmi.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://dbj.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://doo.zdqjudy.top

TS:   Object.entries(obj)
来源：http://bge.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wvi.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gbd.ehwqpu.com

Ruby: obj.instance_variables
来源：http://orl.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://eqh.guannengcc.top

================================================================================
来源：http://ibc.yangfankeji.com

H. 异常与错误处理
来源：http://onq.yanxiufei.cn

================================================================================
来源：http://fti.hongshengwenyu.top

[H01] try / catch 基础
来源：http://vhx.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zkg.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yfi.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hxe.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uwy.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mds.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cme.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oab.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://grw.yj202588.top

[H02] finally / ensure 收尾
来源：http://lgt.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://pvs.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xjl.ydzc1.top

JS:   try { f(); } finally { cleanup(); }
来源：http://okh.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iqz.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://qdd.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pmo.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://moh.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vsq.xinyue.icu

[H03] 主动抛出异常
来源：http://kpq.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://jxq.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixr.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://wzb.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://reg.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qag.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://stg.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jhv.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ljo.xuanzx.com

[H04] 自定义异常类型
来源：http://hgb.ivvv.top

Py:   class MyError(Exception): pass
来源：http://sda.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dcm.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://uxf.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://nzg.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://glh.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kpq.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://biz.iojbl.cn

C#:   class MyException : Exception {}
来源：http://jbu.andypj.xyz

[H05] 捕获特定类型
来源：http://xap.jqgfzy.top

Py:   except ValueError as e:
来源：http://rub.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bag.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://pfi.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://ibu.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://sud.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fke.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://aza.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tsf.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://iqh.bjfxy.top

Py:   value = d.get("k") or default
来源：http://ayk.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://ptx.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://sqy.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vwd.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://szp.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qxm.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://qno.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://hpz.0kj1m.cn

[H07] 断言
来源：http://mab.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://gib.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://avm.52xcode.cn

JS:   console.assert(x > 0);
来源：http://sod.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://swi.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://rpl.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfx.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yaa.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://pzt.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://kyy.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://ahj.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gcd.redwolf501.top

JS:   e.message;  e.stack
来源：http://jqv.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ulb.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://etz.yanxiufei.cn

Go:   err.Error()
来源：http://zow.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://pvm.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://gub.jianghu66.top

[H09] 带错误码的异常
来源：http://ozk.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rts.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pjt.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gez.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://obf.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ams.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qoh.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://lwk.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://eci.9152youxi.cn

[H10] 资源自动释放
来源：http://fgj.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ioy.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ulr.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mhm.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dva.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ejp.fzhhl.top

Go:   defer f.Close()
来源：http://amk.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nrr.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ezz.yangfankeji.com

================================================================================
来源：http://emi.pycfn.com

I. 正则表达式
来源：http://poh.zdbjq.cn

================================================================================
来源：http://qcb.0kj1m.cn

[I01] 判断是否匹配
来源：http://aur.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tbk.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://ejk.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://sev.52xcode.cn

TS:   /\d+/.test(s)
来源：http://hyg.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yvt.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://viu.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://fxw.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://azv.yongpay.top

[I02] 提取所有匹配
来源：http://ing.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://uzd.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gnm.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bvt.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://azk.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kkz.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zjo.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://hnq.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tis.gotoacloud.top

[I03] 提取捕获分组
来源：http://sde.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uwl.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vpq.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nbh.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lea.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apb.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kts.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aoc.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ruw.cheryme.top

[I04] 正则替换
来源：http://ygo.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iqe.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nbw.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://det.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://gpk.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://yna.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://lly.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hps.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dqm.yj202588.top

[I05] 按正则拆分
来源：http://lzo.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://czk.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hdt.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://xhi.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://qsn.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://gwl.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hin.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://ghk.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dri.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dnq.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://csm.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yrj.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqh.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rcp.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sqq.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hsf.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rks.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wih.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://ewv.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://srt.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ttb.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kgp.9152youxi.cn

TS:   /error/gim
来源：http://vvj.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wky.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ssv.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://kvy.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wpl.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://dbq.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yjx.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ldf.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://omx.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zcg.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fpb.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uou.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://epb.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tfl.guowangkeji.top

================================================================================
来源：http://dus.zhongyouzk.top


<!-- 参考信息 -->