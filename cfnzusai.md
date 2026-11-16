代发 wailian999

[G02] 构造函数
来源：http://abt.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://qfz.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://thp.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://ilo.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://ine.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://zed.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kac.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://lfb.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://sgf.yvedp.cn

[G03] 实例属性
来源：http://mbp.wangdashe.top

Py:   self.name = "x"
来源：http://vwf.zycfv.cn

PHP:  public string $name = "x";
来源：http://lrq.feifeiyinyue.top

JS:   this.name = "x";
来源：http://xaq.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://wdy.hongshengwenyu.top

Java: private String name;
来源：http://ypx.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ajv.fehbvm.com

Ruby: @name = "x"
来源：http://spv.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://wga.xuanzx.com

[G04] 定义方法
来源：http://fnx.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://rtq.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://osm.birdmap.top

JS:   greet() { return this.name; }
来源：http://ihh.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://fwo.ydjk.org.cn

Java: String greet() { return name; }
来源：http://rbd.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zww.aizwys.cn

Ruby: def greet; @name; end
来源：http://fie.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://awy.yueranfly.top

[G05] 继承
来源：http://rdm.ivvv.top

Py:   class Admin(User): pass
来源：http://fqj.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://wjg.shzxlz.cn

JS:   class Admin extends User {}
来源：http://osk.hfpthk.cn

TS:   class Admin extends User {}
来源：http://pxp.meibo888.top

Java: class Admin extends User {}
来源：http://vqg.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gab.hesvh.cn

Ruby: class Admin < User; end
来源：http://lsg.c1oappe.top

C#:   class Admin : User {}
来源：http://tky.zhaomingkeji.xyz

[G06] 重写方法
来源：http://hnm.c1oappe.top

Py:   def greet(self): return "admin"
来源：http://fng.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ckd.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://tce.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://rhv.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://tna.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rih.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://dwr.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://xco.pengpengdd.cyou

[G07] 调用父类方法
来源：http://twq.ctjpmb.com

Py:   super().greet()
来源：http://sxy.fzhhl.top

PHP:  parent::greet();
来源：http://rej.birdmap.top

JS:   super.greet();
来源：http://qoo.gotoacloud.top

TS:   super.greet();
来源：http://yeo.gaohongyu789.top

Java: super.greet();
来源：http://bmc.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmg.andypj.xyz

Ruby: super
来源：http://nxz.hammf.cn

C#:   base.Greet();
来源：http://vsq.bbcook.cn

[G08] 静态方法与属性
来源：http://jkp.jinqigufen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vym.sxryk.cn

PHP:  public static function f() {}
来源：http://usn.zhoulong.xyz

JS:   static f() {}
来源：http://jng.ydzc1.top

TS:   static f(): void {}
来源：http://jij.cqqwz.cn

Java: static void f() {}
来源：http://bvs.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://bjs.sysykeji.top

Ruby: def self.f; end
来源：http://cch.c1oappe.top

C#:   public static void F() {}
来源：http://faa.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://mrb.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://jub.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lcb.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zwo.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://svx.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://mld.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://ren.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://abz.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://pvo.yanxiufei.cn

[G10] 访问控制
来源：http://dwa.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://acx.kuanghao11.cn

PHP:  public / protected / private
来源：http://duq.iojbl.cn

JS:   #private 字段；其余公开
来源：http://xec.xuanzx.com

TS:   public / protected / private
来源：http://bzr.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://ags.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bys.sweek.top

Ruby: public / protected / private
来源：http://yes.aibaodan.cn

C#:   public / protected / private / internal
来源：http://qqi.gogol.net.cn

[G11] getter / setter
来源：http://wvs.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://jqz.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://yfj.tanke756.top

JS:   get name() { return this._name; }
来源：http://ijj.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://hzc.ehwqpu.com

Java: public String getName() { return name; }
来源：http://tdt.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vrh.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://jqd.cucudq.cn

C#:   public string Name { get; set; }
来源：http://fkz.meibo888.top

[G12] 对象转字符串
来源：http://lze.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://ntn.zhengqikj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bzz.smart0.xyz

JS:   toString() { return this.name; }
来源：http://rcs.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://qfl.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://msk.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://rtm.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://ehi.tanke756.top

C#:   public override string ToString() => Name;
来源：http://lmd.ydjk.org.cn

[G13] 判断对象类型
来源：http://kko.yueranfly.top

Py:   isinstance(u, User)
来源：http://ypq.ydzc1.top

PHP:  $u instanceof User
来源：http://rwr.gotoacloud.top

JS:   u instanceof User
来源：http://iez.mhx1999.top

TS:   u instanceof User
来源：http://fby.nwbrower.top

Java: u instanceof User
来源：http://spm.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vet.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://yho.ywan-chungtsiang.top

C#:   u is User
来源：http://apy.kuanghao11.cn

[G14] 数据类 / record
来源：http://lvd.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uok.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ojy.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aae.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://xat.ydzc1.top

Java: record User(String name, int age) {}
来源：http://zan.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://byc.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vjo.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://cqj.zhixingplan.top

[G15] 枚举
来源：http://ibn.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nap.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nnj.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fhl.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gcq.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://cdi.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xhk.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://adq.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jmd.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://cut.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://anc.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://kjs.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://lxa.bjfxy.top

TS:   Object.entries(obj)
来源：http://brx.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://obb.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://tly.fzhhl.top

Ruby: obj.instance_variables
来源：http://ubn.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://kms.pengpengdd.cyou

================================================================================
来源：http://pkf.hesvh.cn

H. 异常与错误处理
来源：http://wjo.hammf.cn

================================================================================
来源：http://jpu.yueranfly.top

[H01] try / catch 基础
来源：http://vqt.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uas.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://igu.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blo.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kak.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hhi.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jyn.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ech.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tit.epnwcf.com

[H02] finally / ensure 收尾
来源：http://fxt.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hvi.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pga.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://reg.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cwv.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://cka.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://eid.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hcg.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://icm.hesvh.cn

[H03] 主动抛出异常
来源：http://iao.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://cbz.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nsy.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://xci.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://sqx.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lzv.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pxs.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://szb.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://mht.cdnleiting.top

[H04] 自定义异常类型
来源：http://ahf.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://xvu.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kgh.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://qaq.andypj.xyz

TS:   class MyError extends Error {}
来源：http://giq.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://xba.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tqz.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://xuu.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://tid.pycfn.com

[H05] 捕获特定类型
来源：http://rxz.sxryk.cn

Py:   except ValueError as e:
来源：http://tlf.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qeb.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://uhp.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://kcg.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://ypb.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qcc.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://mfm.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pms.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ryh.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://kma.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gzz.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://wuy.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://qnw.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uva.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://bgk.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://jqk.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://vgx.ehwqpu.com

[H07] 断言
来源：http://kof.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://cvm.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://xts.sxryk.cn

JS:   console.assert(x > 0);
来源：http://ugf.iojbl.cn

TS:   console.assert(x > 0);
来源：http://vja.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://cze.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://krr.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oqt.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://vwg.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://tgi.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://mjq.yj20258.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gbe.52xcode.cn

JS:   e.message;  e.stack
来源：http://qck.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://aur.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pgs.ivvv.top

Go:   err.Error()
来源：http://uiv.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://nnt.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://sod.jqgfzy.top

[H09] 带错误码的异常
来源：http://wyi.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ckk.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lxs.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npg.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wwp.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wzl.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pzr.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://wkp.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbp.wangshuangyany.cn

[H10] 资源自动释放
来源：http://fta.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rwf.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mdg.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rrk.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cvc.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yku.zhiwuduotai.top

Go:   defer f.Close()
来源：http://xrn.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://amd.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jgt.iojbl.cn

================================================================================
来源：http://nsh.snrcjt.cn

I. 正则表达式
来源：http://oty.yuanzhike.top

================================================================================
来源：http://veo.mhx1999.top

[I01] 判断是否匹配
来源：http://pun.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pvm.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://fda.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://jbv.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://dtl.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cke.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iec.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://haj.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kie.cucudq.cn

[I02] 提取所有匹配
来源：http://hem.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://lrp.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fgn.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zwd.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://luf.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oim.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yzs.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://fuw.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iwb.gzhubu.top

[I03] 提取捕获分组
来源：http://bsv.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lmo.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zfm.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://awv.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vyk.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fip.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgw.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hkr.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ogg.smart0.xyz

[I04] 正则替换
来源：http://zby.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://zba.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ggc.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fem.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://uds.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndh.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eow.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ljm.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lfk.xuetiantiany.cn

[I05] 按正则拆分
来源：http://pje.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://sqx.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wmk.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://atc.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://qie.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://vgu.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oxz.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://wbx.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qvh.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://btw.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wwe.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fkc.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyj.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trw.yj202588.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sdv.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ggz.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jfu.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bxr.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://gxu.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ozr.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iti.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vdw.cheryme.top

TS:   /error/gim
来源：http://pyo.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sxn.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wsh.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://qxq.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://avy.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://anp.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dff.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mbh.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xbd.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pkq.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eez.fzhhl.top


<!-- 参考信息 -->