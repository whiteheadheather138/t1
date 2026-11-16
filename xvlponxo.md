代发 wailian999

Java: class User {}
来源：http://aik.yueranfly.top

Go:   type User struct { Name string }
来源：http://vgt.tianlin.xyz

Ruby: class User; end
来源：http://uhm.jinghuilouyu.cn

C#:   class User {}
来源：http://gei.zdbjq.cn

[G02] 构造函数
来源：http://rcl.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://alr.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://hiy.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://zyo.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://zbf.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://sra.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bng.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://wpb.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://zus.zhixingplan.top

[G03] 实例属性
来源：http://mid.tianlin.xyz

Py:   self.name = "x"
来源：http://jvy.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://vql.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://nfz.sjlbkw.cn

TS:   name: string = "x";
来源：http://zbx.aibaodan.cn

Java: private String name;
来源：http://atq.cqqwz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hng.ehwqpu.com

Ruby: @name = "x"
来源：http://xbj.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ids.yfazqb.com

[G04] 定义方法
来源：http://gyp.hcnkem.com

Py:   def greet(self): return self.name
来源：http://isv.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ykt.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://zgl.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://ixp.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://nji.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://edc.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://ngk.sysykeji.top

C#:   public string Greet() => Name;
来源：http://ihx.daxiang520.top

[G05] 继承
来源：http://and.fzhhl.top

Py:   class Admin(User): pass
来源：http://xyl.ybcxt.top

PHP:  class Admin extends User {}
来源：http://tsn.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://wdk.0kj1m.cn

TS:   class Admin extends User {}
来源：http://gyl.xziqi.cn

Java: class Admin extends User {}
来源：http://sjy.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nsf.dashuyun.cn

Ruby: class Admin < User; end
来源：http://zar.yangfankeji.com

C#:   class Admin : User {}
来源：http://ian.pengpengdd.cyou

[G06] 重写方法
来源：http://qut.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://agx.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dyp.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://yts.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://pci.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kqi.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://glv.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://qnj.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://goh.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://gsz.birdmap.top

Py:   super().greet()
来源：http://yac.yuanzhike.top

PHP:  parent::greet();
来源：http://lnb.hongshengwenyu.top

JS:   super.greet();
来源：http://fij.nwbrower.top

TS:   super.greet();
来源：http://lak.zhaomingkeji.xyz

Java: super.greet();
来源：http://wup.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cod.shuidangran.top

Ruby: super
来源：http://hlm.yj20258.top

C#:   base.Greet();
来源：http://wvh.gotoacloud.top

[G08] 静态方法与属性
来源：http://pis.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zoi.0kj1m.cn

PHP:  public static function f() {}
来源：http://fxn.yuanzhike.top

JS:   static f() {}
来源：http://etk.fengsongda.top

TS:   static f(): void {}
来源：http://xpx.daria6918.cn

Java: static void f() {}
来源：http://ykb.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://usk.sjlbkw.cn

Ruby: def self.f; end
来源：http://ebm.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://jga.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://bpe.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://ife.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rjv.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uqs.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://gus.sweek.top

Java: interface Shape { double area(); }
来源：http://arm.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://xbc.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zlq.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://jmg.fktsv.cn

[G10] 访问控制
来源：http://fzi.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://mlk.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://yox.fktsv.cn

JS:   #private 字段；其余公开
来源：http://opp.zhixingplan.top

TS:   public / protected / private
来源：http://pxs.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://gld.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nhp.yj20258.top

Ruby: public / protected / private
来源：http://oid.epnwcf.com

C#:   public / protected / private / internal
来源：http://nzw.yj20258888.top

[G11] getter / setter
来源：http://qze.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://qqk.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mvo.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://vkf.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://fpz.andypj.xyz

Java: public String getName() { return name; }
来源：http://cxi.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://spp.smart0.xyz

Ruby: attr_accessor :name
来源：http://xxt.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://qcn.hysaishi.cn

[G12] 对象转字符串
来源：http://fzf.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://fsv.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bat.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://gyd.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://sya.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://pwm.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://dow.tarul.cn

Ruby: def to_s; @name; end
来源：http://sfg.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://qol.snrcjt.cn

[G13] 判断对象类型
来源：http://udb.tian-w.cn

Py:   isinstance(u, User)
来源：http://dup.pycfn.com

PHP:  $u instanceof User
来源：http://gqw.haohaochexian.top

JS:   u instanceof User
来源：http://emn.hnxiangtu.top

TS:   u instanceof User
来源：http://rvr.iojbl.cn

Java: u instanceof User
来源：http://shd.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dmq.fehbvm.com

Ruby: u.is_a?(User)
来源：http://vht.iojbl.cn

C#:   u is User
来源：http://ssy.sysykeji.top

[G14] 数据类 / record
来源：http://kqd.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jry.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://jip.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xfo.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://kne.fzhhl.top

Java: record User(String name, int age) {}
来源：http://ujz.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://bma.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ucg.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://wdz.yuanzhike.top

[G15] 枚举
来源：http://jqv.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rvf.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lwn.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fog.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zhw.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://elv.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kfz.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://ggz.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zfs.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://ghz.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://umy.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://mih.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://esl.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://cwn.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lbj.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mok.fktsv.cn

Ruby: obj.instance_variables
来源：http://tch.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://kmd.shangyingyoupin.top

================================================================================
来源：http://vry.sysykeji.top

H. 异常与错误处理
来源：http://rom.hnqzz.top

================================================================================
来源：http://ufq.jinqigufen.top

[H01] try / catch 基础
来源：http://nnq.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fsc.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dbz.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mte.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pna.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tdr.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wgy.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xtn.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ptj.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://hfe.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://ovc.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://nkn.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://njw.zhaomingkeji.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://gru.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://uww.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xbx.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pep.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://whl.gogol.net.cn

[H03] 主动抛出异常
来源：http://yet.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://bdb.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://axs.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://aiq.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://ves.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://abm.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sxz.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gpi.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://gjh.ydjk.org.cn

[H04] 自定义异常类型
来源：http://poz.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://yey.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://zyx.gzhubu.top

JS:   class MyError extends Error {}
来源：http://sts.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://rco.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://mzn.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eee.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://wyd.yj20258888.top

C#:   class MyException : Exception {}
来源：http://tdz.dashuyun.cn

[H05] 捕获特定类型
来源：http://tgt.yfazqb.com

Py:   except ValueError as e:
来源：http://mvx.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uyp.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://hup.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://uep.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://dqc.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qfo.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://osa.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tkg.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://fou.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://cra.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gkk.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pgr.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://tqw.dashuyun.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sks.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nik.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://bzy.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://jfj.0kj1m.cn

[H07] 断言
来源：http://mem.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://hsu.sufxvd.cn

PHP:  assert($x > 0);
来源：http://atw.zhiwuduotai.top

JS:   console.assert(x > 0);
来源：http://zdj.andypj.xyz

TS:   console.assert(x > 0);
来源：http://srr.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://bxb.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://loq.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lxs.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://imb.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://plp.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://qhm.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://upm.andypj.xyz

JS:   e.message;  e.stack
来源：http://etq.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://bcf.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nci.pengpengdd.cyou

Go:   err.Error()
来源：http://yvm.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://wxi.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://dxm.yuxming.cn

[H09] 带错误码的异常
来源：http://ecj.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kac.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uwo.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qqf.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tre.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bci.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ivz.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://wsx.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gxv.guannengcc.top

[H10] 资源自动释放
来源：http://pru.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ixa.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jcg.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xhs.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://amh.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dpp.ybcxt.top

Go:   defer f.Close()
来源：http://pby.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://czg.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cdo.shanyushiyangkeji.top

================================================================================
来源：http://usc.redwolf501.top

I. 正则表达式
来源：http://dur.sysykeji.top

================================================================================
来源：http://moc.gotoacloud.top

[I01] 判断是否匹配
来源：http://rxz.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lmo.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fim.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://slr.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://wrd.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xqy.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qke.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://vlm.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gzh.gogol.net.cn

[I02] 提取所有匹配
来源：http://hxt.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://zfv.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fuc.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fik.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://bps.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qxr.xylfe.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vbe.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://ixm.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://epq.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://jnd.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dka.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rau.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jta.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wkw.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dmz.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oup.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://asv.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://noh.zhengqikj.top

[I04] 正则替换
来源：http://azu.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://vhc.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hat.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://xtu.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://zzv.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ydw.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://eck.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://svi.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xrx.pycfn.com

[I05] 按正则拆分
来源：http://nll.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ral.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iib.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://izh.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://mlh.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://ykl.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dlr.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://jzm.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zwn.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hmc.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gov.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ejh.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://thn.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxg.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aux.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tsw.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zsm.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ayw.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://eew.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://otk.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tgm.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://peb.havefunace.top

TS:   /error/gim
来源：http://dzq.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ayy.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jgt.hammf.cn

Ruby: s.scan(/error/i)
来源：http://yoz.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://teh.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://fbf.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://csh.gaohongyu789.top


<!-- 参考信息 -->