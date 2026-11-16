代发 wailian999

TS:   constructor(public name: string) {}
来源：http://sca.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://ozo.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://clq.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://zew.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://pek.jinqigfzy.top

[G03] 实例属性
来源：http://gsw.havefunace.top

Py:   self.name = "x"
来源：http://kgv.yj202588.top

PHP:  public string $name = "x";
来源：http://jbx.fehbvm.com

JS:   this.name = "x";
来源：http://wli.daxiang520.top

TS:   name: string = "x";
来源：http://swb.cucudq.cn

Java: private String name;
来源：http://uzc.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hry.sjlbkw.cn

Ruby: @name = "x"
来源：http://oth.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://ioa.uphjek.com

[G04] 定义方法
来源：http://neg.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://tzh.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://soj.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://lpo.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://ykh.birdmap.top

Java: String greet() { return name; }
来源：http://whs.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sff.jinqigufen.top

Ruby: def greet; @name; end
来源：http://ujl.cashguo.top

C#:   public string Greet() => Name;
来源：http://ysp.hysaishi.cn

[G05] 继承
来源：http://lnq.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://hfm.birdmap.top

PHP:  class Admin extends User {}
来源：http://pcs.jiagoushi.top

JS:   class Admin extends User {}
来源：http://cpn.snrcjt.cn

TS:   class Admin extends User {}
来源：http://hhu.cqqwz.cn

Java: class Admin extends User {}
来源：http://ypd.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywp.yj20258.top

Ruby: class Admin < User; end
来源：http://wcf.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://ewy.pengpengdd.cyou

[G06] 重写方法
来源：http://swi.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://kdu.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mev.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://anh.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://war.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://hrn.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nfv.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://hve.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://enh.yuxming.cn

[G07] 调用父类方法
来源：http://tjh.guowangkeji.top

Py:   super().greet()
来源：http://acd.dianchejie.cn

PHP:  parent::greet();
来源：http://zut.yanxiufei.cn

JS:   super.greet();
来源：http://rmx.xziqi.cn

TS:   super.greet();
来源：http://xtn.cashguo.top

Java: super.greet();
来源：http://bpt.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ztc.ehwqpu.com

Ruby: super
来源：http://nhj.xylfe.cn

C#:   base.Greet();
来源：http://mgt.tanke756.top

[G08] 静态方法与属性
来源：http://enh.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pjx.jlsjyb.cn

PHP:  public static function f() {}
来源：http://xeo.jinyuanbaomall.cn

JS:   static f() {}
来源：http://npb.tarul.cn

TS:   static f(): void {}
来源：http://reo.fehbvm.com

Java: static void f() {}
来源：http://tlf.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://gtl.zhixingplan.top

Ruby: def self.f; end
来源：http://pae.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://llf.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://deo.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://wfn.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://ulm.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zut.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://emu.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://qms.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://gcp.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jbj.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://pzr.0kj1m.cn

[G10] 访问控制
来源：http://jcx.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://aiq.nwbrower.top

PHP:  public / protected / private
来源：http://lrz.yj202588.top

JS:   #private 字段；其余公开
来源：http://vsi.meibo888.top

TS:   public / protected / private
来源：http://fin.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://gji.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ilg.bjfxy.top

Ruby: public / protected / private
来源：http://rnn.yj202588.top

C#:   public / protected / private / internal
来源：http://ctn.meibo888.top

[G11] getter / setter
来源：http://krx.xinyue.icu

Py:   @property 与 @x.setter
来源：http://cpw.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sbh.ivvv.top

JS:   get name() { return this._name; }
来源：http://wqb.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://vpy.cucudq.cn

Java: public String getName() { return name; }
来源：http://dcs.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://urw.gzhubu.top

Ruby: attr_accessor :name
来源：http://isr.epnwcf.com

C#:   public string Name { get; set; }
来源：http://dke.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://jbn.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://fub.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://keu.yueranfly.top

JS:   toString() { return this.name; }
来源：http://yxn.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://jgv.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://fht.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://pnf.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://xot.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://ccn.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://etv.fzhhl.top

Py:   isinstance(u, User)
来源：http://pbm.cdnleiting.top

PHP:  $u instanceof User
来源：http://fhl.jinqigufen.top

JS:   u instanceof User
来源：http://fhk.birdmap.top

TS:   u instanceof User
来源：http://xjp.bjfxy.top

Java: u instanceof User
来源：http://awb.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ewm.sysykeji.top

Ruby: u.is_a?(User)
来源：http://rnn.daria6918.cn

C#:   u is User
来源：http://rdr.yuanzhike.top

[G14] 数据类 / record
来源：http://zhx.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://spe.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://tyd.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://byz.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://ljb.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://vup.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://cuo.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jeg.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://gau.ybcxt.top

[G15] 枚举
来源：http://odq.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dqs.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qff.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yew.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npt.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://qaf.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lhc.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://hqd.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kra.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://pdr.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bgf.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://oyl.redwolf501.top

JS:   Object.entries(obj)
来源：http://efv.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://hzv.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hbi.cdnleiting.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zyz.yongpay.top

Ruby: obj.instance_variables
来源：http://srn.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://oho.9152youxi.cn

================================================================================
来源：http://zhb.xuetiantiany.cn

H. 异常与错误处理
来源：http://hwo.meibo888.top

================================================================================
来源：http://fbg.tianlin.xyz

[H01] try / catch 基础
来源：http://xez.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jyt.zhoulong.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ngu.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bgd.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jxm.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://voh.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ort.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fhc.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kgj.gzhubu.top

[H02] finally / ensure 收尾
来源：http://pdj.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zyk.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nbc.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://axz.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dtz.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://qwr.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cqk.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://niz.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gcg.cucudq.cn

[H03] 主动抛出异常
来源：http://pac.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://btz.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lkm.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://cov.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://cva.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gel.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sca.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gng.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ryj.snrcjt.cn

[H04] 自定义异常类型
来源：http://div.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://wah.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://rvs.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://xec.redwolf501.top

TS:   class MyError extends Error {}
来源：http://grx.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://kam.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jfn.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://ffk.yvedp.cn

C#:   class MyException : Exception {}
来源：http://tlh.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://kxm.ppjwa.cn

Py:   except ValueError as e:
来源：http://xwx.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ncw.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://ebg.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://evo.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://lhy.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gyx.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://amz.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://emj.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://wnp.hcnkem.com

Py:   value = d.get("k") or default
来源：http://nlv.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://bik.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://guw.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://mmu.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://saa.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sut.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://hhd.sjlbkw.cn

C#:   obj?.A?.B ?? default
来源：http://uso.yuxming.cn

[H07] 断言
来源：http://soa.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://hce.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://exb.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://yge.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://wrm.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://zsw.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fqi.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tww.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://cpi.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://zrj.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://agy.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rjf.hysaishi.cn

JS:   e.message;  e.stack
来源：http://byl.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lsm.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wwa.tarul.cn

Go:   err.Error()
来源：http://hoi.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://dbl.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://yyd.ctjpmb.com

[H09] 带错误码的异常
来源：http://rsq.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zqj.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rap.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lzd.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qot.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baj.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uyh.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://dze.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wfn.xuanzx.com

[H10] 资源自动释放
来源：http://ici.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmh.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fch.fzhhl.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fos.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tla.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tgt.cqqwz.cn

Go:   defer f.Close()
来源：http://yfd.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ffa.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cny.cdnleiting.top

================================================================================
来源：http://btc.9152youxi.cn

I. 正则表达式
来源：http://yyn.feifeiyinyue.top

================================================================================
来源：http://ymt.zhijiandao.cn

[I01] 判断是否匹配
来源：http://kur.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ftq.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://ldw.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://zge.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://eet.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cje.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://efc.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://myi.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pec.ydjk.org.cn

[I02] 提取所有匹配
来源：http://rtb.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://vwc.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kab.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xrz.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://smk.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wkx.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ncm.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://qmc.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbq.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://rvw.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gfu.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bfs.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hxa.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zdj.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gfi.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://txv.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wpi.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eqq.sufxvd.cn

[I04] 正则替换
来源：http://ajh.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pzd.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eml.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://gif.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://idf.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://qri.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://adi.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dnk.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://htp.feifeiyinyue.top

[I05] 按正则拆分
来源：http://jrz.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ook.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nru.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://isb.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://gwy.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://pvu.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dug.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://fky.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tuq.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://exp.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvb.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cmh.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyb.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukw.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://frc.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tbk.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xin.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsf.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://jvv.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yvi.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wwq.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xtx.dashuyun.cn

TS:   /error/gim
来源：http://ldu.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://krb.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yzs.tanke756.top

Ruby: s.scan(/error/i)
来源：http://vlh.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntn.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://ptl.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ezr.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yla.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bck.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tve.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://olh.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qvn.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nar.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://swd.jyoumei.cn

================================================================================
来源：http://fty.daxiang520.top


<!-- 参考信息 -->