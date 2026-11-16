代发 wailian999

TS:   constructor(public name: string) {}
来源：http://txm.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://zba.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://psy.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://dnk.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://rev.hammf.cn

[G03] 实例属性
来源：http://kgc.zdqjudy.top

Py:   self.name = "x"
来源：http://rfl.fktsv.cn

PHP:  public string $name = "x";
来源：http://zaw.aibaodan.cn

JS:   this.name = "x";
来源：http://aja.ppjwa.cn

TS:   name: string = "x";
来源：http://yxi.cheryme.top

Java: private String name;
来源：http://gan.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://spr.chenlongwang.top

Ruby: @name = "x"
来源：http://jzl.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://pwc.jyoumei.cn

[G04] 定义方法
来源：http://wim.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://vhn.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://iei.yongpay.top

JS:   greet() { return this.name; }
来源：http://ocp.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://ist.daria6918.cn

Java: String greet() { return name; }
来源：http://wpr.jinyuanbaomall.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yxs.vehdjk.com

Ruby: def greet; @name; end
来源：http://rav.cheryme.top

C#:   public string Greet() => Name;
来源：http://zgd.hongshengwenyu.top

[G05] 继承
来源：http://xza.hysaishi.cn

Py:   class Admin(User): pass
来源：http://iqm.cucudq.cn

PHP:  class Admin extends User {}
来源：http://mgz.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://cmc.mhx1999.top

TS:   class Admin extends User {}
来源：http://awo.aibaodan.cn

Java: class Admin extends User {}
来源：http://qzg.cucudq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://laa.jqgfzy.top

Ruby: class Admin < User; end
来源：http://aga.ybcxt.top

C#:   class Admin : User {}
来源：http://tuz.9152youxi.cn

[G06] 重写方法
来源：http://oki.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://fyv.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://epm.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://zde.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://tuh.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://xfa.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ror.ivvv.top

Ruby: def greet; "admin"; end
来源：http://qcc.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://oyr.sufxvd.cn

[G07] 调用父类方法
来源：http://qhe.tianlin.xyz

Py:   super().greet()
来源：http://vfv.nwbrower.top

PHP:  parent::greet();
来源：http://fge.gogol.net.cn

JS:   super.greet();
来源：http://sml.aibaodan.cn

TS:   super.greet();
来源：http://veo.jiagoushi.top

Java: super.greet();
来源：http://aqd.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ctv.fzhhl.top

Ruby: super
来源：http://kui.fehbvm.com

C#:   base.Greet();
来源：http://zmu.zhongyouzk.top

[G08] 静态方法与属性
来源：http://ztg.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hct.sjlbkw.cn

PHP:  public static function f() {}
来源：http://iiq.xuetiantiany.cn

JS:   static f() {}
来源：http://bgn.xinyue.icu

TS:   static f(): void {}
来源：http://rah.jlsjyb.cn

Java: static void f() {}
来源：http://vsh.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zjx.tanke756.top

Ruby: def self.f; end
来源：http://mrk.sjlbkw.cn

C#:   public static void F() {}
来源：http://tmn.52xcode.cn

[G09] 接口 / 抽象类
来源：http://qnc.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://pek.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://jvb.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ukx.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://tsd.cheryme.top

Java: interface Shape { double area(); }
来源：http://tcp.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://rdi.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ind.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://yew.xziqi.cn

[G10] 访问控制
来源：http://bzs.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://phy.aibaodan.cn

PHP:  public / protected / private
来源：http://cik.smart0.xyz

JS:   #private 字段；其余公开
来源：http://nxa.zdbjq.cn

TS:   public / protected / private
来源：http://irx.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://mhf.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aen.jqgfzy.top

Ruby: public / protected / private
来源：http://avf.ybcxt.top

C#:   public / protected / private / internal
来源：http://nzp.svipenyu.cn

[G11] getter / setter
来源：http://uku.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://edr.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tle.andypj.xyz

JS:   get name() { return this._name; }
来源：http://lup.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://jgk.fehbvm.com

Java: public String getName() { return name; }
来源：http://wkh.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tjl.vehdjk.com

Ruby: attr_accessor :name
来源：http://osf.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://zyg.zhoulong.xyz

[G12] 对象转字符串
来源：http://dld.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://uhc.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ayk.ydzc1.top

JS:   toString() { return this.name; }
来源：http://awt.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://gtf.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://vtc.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fdq.bjfxy.top

Ruby: def to_s; @name; end
来源：http://ohz.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://bgm.daria6918.cn

[G13] 判断对象类型
来源：http://puu.tarul.cn

Py:   isinstance(u, User)
来源：http://ezw.cheryme.top

PHP:  $u instanceof User
来源：http://exn.yuxming.cn

JS:   u instanceof User
来源：http://xgg.shzxlz.cn

TS:   u instanceof User
来源：http://qqv.uphjek.com

Java: u instanceof User
来源：http://lua.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lpo.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://pzw.jinqigufen.top

C#:   u is User
来源：http://epu.tianlin.xyz

[G14] 数据类 / record
来源：http://reg.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ade.hnqzz.top

PHP:  // 用 readonly 属性模拟
来源：http://vsk.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://stp.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://vjw.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://acw.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://xwt.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://umf.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://nhu.guannengcc.top

[G15] 枚举
来源：http://obr.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ymf.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://qnj.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zqv.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ctj.316326.xyz

Java: enum Color { RED, GREEN }
来源：http://pzq.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rkl.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://ftd.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lfd.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://yvm.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zhy.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://pbp.wangdashe.top

JS:   Object.entries(obj)
来源：http://xdf.0kj1m.cn

TS:   Object.entries(obj)
来源：http://pjz.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://efa.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tlp.cqqwz.cn

Ruby: obj.instance_variables
来源：http://cmu.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://kcd.jyoumei.cn

================================================================================
来源：http://izr.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://syr.shangyingyoupin.top

================================================================================
来源：http://khx.ppjwa.cn

[H01] try / catch 基础
来源：http://xfj.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qho.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jzc.sxryk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ptl.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://doy.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://omz.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sqm.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xck.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zzg.xylfe.cn

[H02] finally / ensure 收尾
来源：http://umt.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://ocn.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ros.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vgs.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mgc.hysaishi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xgm.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mkr.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dof.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vdy.9152youxi.cn

[H03] 主动抛出异常
来源：http://mkp.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://vjy.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mwm.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://ahj.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://veq.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qbd.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mgd.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ker.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://ymd.guannengcc.top

[H04] 自定义异常类型
来源：http://sqx.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://lbe.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://jml.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://twe.yvedp.cn

TS:   class MyError extends Error {}
来源：http://npt.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://pil.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mxi.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://nbw.yuxming.cn

C#:   class MyException : Exception {}
来源：http://mlx.gzhubu.top

[H05] 捕获特定类型
来源：http://hoj.zdqjudy.top

Py:   except ValueError as e:
来源：http://pnz.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bya.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://iuw.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://aov.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://rhf.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://egy.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://cvw.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bus.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://ntg.bbcook.cn

Py:   value = d.get("k") or default
来源：http://uai.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://kuo.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://whq.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cif.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ctp.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fcj.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://qkp.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://xou.xuanzx.com

[H07] 断言
来源：http://mxj.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://hil.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://blt.smart0.xyz

JS:   console.assert(x > 0);
来源：http://xnp.cashguo.top

TS:   console.assert(x > 0);
来源：http://xwv.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://zdd.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vsk.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://dhh.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://qqm.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://hok.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://yzg.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ecf.shzxlz.cn

JS:   e.message;  e.stack
来源：http://oic.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://fny.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jjj.shanyushiyangtech.top

Go:   err.Error()
来源：http://erb.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://oam.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://omm.hcnkem.com

[H09] 带错误码的异常
来源：http://gls.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://acg.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vjg.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xkj.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lzv.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tsg.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rpr.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://rfz.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kdz.vehdjk.com

[H10] 资源自动释放
来源：http://bzw.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pgv.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oga.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lxv.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ahe.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ncd.nanxinkj.top

Go:   defer f.Close()
来源：http://mus.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://snk.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dmk.cheryme.top

================================================================================
来源：http://onc.ydzc1.top

I. 正则表达式
来源：http://bmw.cashguo.top

================================================================================
来源：http://cyj.jyoumei.cn

[I01] 判断是否匹配
来源：http://stx.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzb.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kjx.yonumen.top

JS:   /\d+/.test(s)
来源：http://bpb.fktsv.cn

TS:   /\d+/.test(s)
来源：http://aom.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lqt.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hye.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://tbd.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqq.tanke756.top

[I02] 提取所有匹配
来源：http://dlf.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://hmv.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oxo.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kje.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://per.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uht.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ocw.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://sou.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ubu.zhoulong.xyz

[I03] 提取捕获分组
来源：http://ven.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uuq.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://obw.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dvw.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bpp.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tmi.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jsv.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ueg.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pzb.cheryme.top

[I04] 正则替换
来源：http://yem.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pff.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xkd.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nyj.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yna.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://amy.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kvb.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wwt.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://leh.sweek.top

[I05] 按正则拆分
来源：http://dka.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://brd.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jrc.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://zen.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://clu.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://htd.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bkg.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://bnx.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://syl.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kpe.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://abc.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hmb.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://akw.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vff.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://opl.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qwr.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rga.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ssd.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://rra.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ony.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kit.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lud.nanxinkj.top

TS:   /error/gim
来源：http://std.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aoe.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xqt.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://lvu.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kjg.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://yok.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://adj.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ags.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hvn.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hhl.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jyp.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uzw.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://deh.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sgi.vqdsnc.cn

================================================================================
来源：http://ipe.mhx1999.top


<!-- 参考信息 -->