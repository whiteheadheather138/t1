代发 wailian999

[G02] 构造函数
来源：http://hbh.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://lgs.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://jkm.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://dgp.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://vlw.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://oxd.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obg.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://pdv.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://blc.quarkkingdee.top

[G03] 实例属性
来源：http://ebv.52xcode.cn

Py:   self.name = "x"
来源：http://khc.xylfe.cn

PHP:  public string $name = "x";
来源：http://lzt.ivvv.top

JS:   this.name = "x";
来源：http://kuc.xuetiantiany.cn

TS:   name: string = "x";
来源：http://gpb.ppjwa.cn

Java: private String name;
来源：http://ehi.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://myb.yuanzhike.top

Ruby: @name = "x"
来源：http://khs.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://zlu.jinghuilouyu.cn

[G04] 定义方法
来源：http://geo.yonumen.top

Py:   def greet(self): return self.name
来源：http://zge.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lhv.daria6918.cn

JS:   greet() { return this.name; }
来源：http://flf.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://xxb.bjfxy.top

Java: String greet() { return name; }
来源：http://omx.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://eij.yonumen.top

Ruby: def greet; @name; end
来源：http://pvf.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://ttx.feifeiyinyue.top

[G05] 继承
来源：http://uvm.hcnkem.com

Py:   class Admin(User): pass
来源：http://vjo.vehdjk.com

PHP:  class Admin extends User {}
来源：http://adz.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://row.hywenlv.cn

TS:   class Admin extends User {}
来源：http://tlc.ppjwa.cn

Java: class Admin extends User {}
来源：http://lqy.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lnz.sweek.top

Ruby: class Admin < User; end
来源：http://rta.xinyue.icu

C#:   class Admin : User {}
来源：http://jee.ehwqpu.com

[G06] 重写方法
来源：http://mwn.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://bkt.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://did.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://ttx.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://nvb.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://ijq.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ttk.yongpay.top

Ruby: def greet; "admin"; end
来源：http://xcg.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://ztn.yuxming.cn

[G07] 调用父类方法
来源：http://pzd.yvedp.cn

Py:   super().greet()
来源：http://zxw.feifeiyinyue.top

PHP:  parent::greet();
来源：http://fix.xziqi.cn

JS:   super.greet();
来源：http://svg.chenlongwang.top

TS:   super.greet();
来源：http://jnn.xinyue.icu

Java: super.greet();
来源：http://ckk.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pfk.guannengcc.top

Ruby: super
来源：http://cnr.ivvv.top

C#:   base.Greet();
来源：http://kli.jinqigfzy.top

[G08] 静态方法与属性
来源：http://ouc.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qgs.guowangkeji.top

PHP:  public static function f() {}
来源：http://boy.gotoacloud.top

JS:   static f() {}
来源：http://twz.0kj1m.cn

TS:   static f(): void {}
来源：http://xxu.cheryme.top

Java: static void f() {}
来源：http://pcc.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://exf.ydjk.org.cn

Ruby: def self.f; end
来源：http://tyi.yfazqb.com

C#:   public static void F() {}
来源：http://mst.wangdashe.top

[G09] 接口 / 抽象类
来源：http://qkp.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://hjk.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ryx.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kub.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://qdu.52xcode.cn

Java: interface Shape { double area(); }
来源：http://chb.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://nqv.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xoi.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://tha.tanke756.top

[G10] 访问控制
来源：http://fmv.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://bbe.xuanzx.com

PHP:  public / protected / private
来源：http://myx.fengsongda.top

JS:   #private 字段；其余公开
来源：http://iuf.nanxuanxn.top

TS:   public / protected / private
来源：http://dck.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://kiz.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rfs.hfpthk.cn

Ruby: public / protected / private
来源：http://zkx.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://noo.andypj.xyz

[G11] getter / setter
来源：http://eee.yj202588.top

Py:   @property 与 @x.setter
来源：http://pja.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jar.aizwys.cn

JS:   get name() { return this._name; }
来源：http://vls.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://hhj.guowangkeji.top

Java: public String getName() { return name; }
来源：http://cph.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dub.havefunace.top

Ruby: attr_accessor :name
来源：http://gwa.aizwys.cn

C#:   public string Name { get; set; }
来源：http://fmu.jiagoushi.top

[G12] 对象转字符串
来源：http://fcw.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://yrm.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://utr.epnwcf.com

JS:   toString() { return this.name; }
来源：http://kas.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://qlz.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://akb.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://nyi.316326.xyz

Ruby: def to_s; @name; end
来源：http://dke.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://zbd.tanke756.top

[G13] 判断对象类型
来源：http://jat.tian-w.cn

Py:   isinstance(u, User)
来源：http://tuf.tian-w.cn

PHP:  $u instanceof User
来源：http://rui.hnxiangtu.top

JS:   u instanceof User
来源：http://nlg.52xcode.cn

TS:   u instanceof User
来源：http://zvu.yj202588.top

Java: u instanceof User
来源：http://vpm.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mvo.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://iuj.fktsv.cn

C#:   u is User
来源：http://ekv.hnqzz.top

[G14] 数据类 / record
来源：http://npo.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qoh.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://cqk.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://fwa.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://csh.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://eua.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://smh.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zkz.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://wqy.jinqigufen.top

[G15] 枚举
来源：http://dny.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tev.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dgp.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mqr.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fhe.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://nup.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xxa.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://mfi.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zln.yj202588.top

[G16] 对象转数组 / 字典
来源：http://gks.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mec.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://pwn.andypj.xyz

JS:   Object.entries(obj)
来源：http://jde.tian-w.cn

TS:   Object.entries(obj)
来源：http://gic.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://phz.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://agm.sysykeji.top

Ruby: obj.instance_variables
来源：http://gms.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://sjs.cashguo.top

================================================================================
来源：http://cxe.guowangkeji.top

H. 异常与错误处理
来源：http://lgz.cucudq.cn

================================================================================
来源：http://xxv.316326.xyz

[H01] try / catch 基础
来源：http://zwr.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cnh.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aff.nanxinkj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kmt.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pjg.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ixb.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pje.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oqq.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qut.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://lsn.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://jlb.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://etu.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dba.zhaomingkeji.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zhw.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://jvv.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozt.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vhe.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oda.zhoulong.xyz

[H03] 主动抛出异常
来源：http://occ.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://scn.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cle.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://ner.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://wix.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rxe.andypj.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lyw.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://erx.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://fnr.zycfv.cn

[H04] 自定义异常类型
来源：http://abt.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://tvd.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://grm.redwolf501.top

JS:   class MyError extends Error {}
来源：http://fim.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://rzm.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://fmo.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ual.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://his.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://kdj.jqgufenzy.top

[H05] 捕获特定类型
来源：http://lgd.jqgfzy.top

Py:   except ValueError as e:
来源：http://ams.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uql.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://umj.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wey.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://qgv.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yxi.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://lyq.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgm.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://yha.bjfxy.top

Py:   value = d.get("k") or default
来源：http://xkp.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://tiy.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://uxn.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://kov.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nmf.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fjw.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://pkh.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://dbx.hesvh.cn

[H07] 断言
来源：http://cao.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://erw.zdbjq.cn

PHP:  assert($x > 0);
来源：http://iaz.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://cat.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://bns.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://znr.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jpq.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vbk.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://zrx.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://quj.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://spg.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbn.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://lew.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfc.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ssa.zhiwuduotai.top

Go:   err.Error()
来源：http://sbp.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://wge.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://jkt.zdbjq.cn

[H09] 带错误码的异常
来源：http://nzi.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://stm.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qzw.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxj.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tco.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tnh.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://shs.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dpj.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zdm.tanke756.top

[H10] 资源自动释放
来源：http://pvo.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://lqt.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://orw.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rfe.9152youxi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hfj.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rmv.ivvv.top

Go:   defer f.Close()
来源：http://nbm.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://stz.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdm.cucudq.cn

================================================================================
来源：http://cbr.shzxlz.cn

I. 正则表达式
来源：http://ymk.hesvh.cn

================================================================================
来源：http://kot.c1oappe.top

[I01] 判断是否匹配
来源：http://maj.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://otu.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yht.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://slt.fktsv.cn

TS:   /\d+/.test(s)
来源：http://myq.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jpe.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aju.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://mqd.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xys.fehbvm.com

[I02] 提取所有匹配
来源：http://wqg.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://jno.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ygi.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://itb.yonumen.top

TS:   s.match(/\d+/g)
来源：http://ydb.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sun.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cbp.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://nbn.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vkd.birdmap.top

[I03] 提取捕获分组
来源：http://guj.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dbt.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://whm.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oaz.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qcm.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kng.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bkn.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://slo.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ncp.hnxiangtu.top

[I04] 正则替换
来源：http://zub.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vyf.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://exo.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ngj.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://wos.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nxs.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yuz.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dsa.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ftw.ehwqpu.com

[I05] 按正则拆分
来源：http://ndm.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://oqx.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vmi.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://gav.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://pch.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://efg.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dre.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qhj.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgx.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tmm.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qfy.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jbc.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aow.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgz.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iqr.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jyu.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ykf.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tbt.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://mwq.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xsh.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nnl.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://swx.zhijiandao.cn

TS:   /error/gim
来源：http://ald.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lkp.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://enn.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://yoi.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://beg.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://yzy.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ubb.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wic.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmt.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ayr.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gxj.smart0.xyz


<!-- 参考信息 -->