代发 wailian999

TS:   constructor(public name: string) {}
来源：http://cda.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://rma.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rjy.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://lex.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://gtt.gzhubu.top

[G03] 实例属性
来源：http://ybj.tianlin.xyz

Py:   self.name = "x"
来源：http://oql.yfazqb.com

PHP:  public string $name = "x";
来源：http://ghu.zhiwuduotai.top

JS:   this.name = "x";
来源：http://spa.xingfuxueyuan.xyz

TS:   name: string = "x";
来源：http://bey.hnqzz.top

Java: private String name;
来源：http://bvw.jinyuanbaomall.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hvn.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://rac.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://gmg.jqgfzy.top

[G04] 定义方法
来源：http://eia.hnqzz.top

Py:   def greet(self): return self.name
来源：http://cvb.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pjx.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://bil.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://ocs.hnxiangtu.top

Java: String greet() { return name; }
来源：http://mbx.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yds.fengsongda.top

Ruby: def greet; @name; end
来源：http://kji.daxiang520.top

C#:   public string Greet() => Name;
来源：http://wap.zycfv.cn

[G05] 继承
来源：http://mmt.svipenyu.cn

Py:   class Admin(User): pass
来源：http://yay.uphjek.com

PHP:  class Admin extends User {}
来源：http://fxr.zdbjq.cn

JS:   class Admin extends User {}
来源：http://xxg.chenzaomai.com

TS:   class Admin extends User {}
来源：http://yey.quarkkingdee.top

Java: class Admin extends User {}
来源：http://myz.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qzr.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://ucy.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://elt.vqdsnc.cn

[G06] 重写方法
来源：http://rmg.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://cfg.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tkr.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://wjl.jinqigufen.top

TS:   greet(): string { return "admin"; }
来源：http://coq.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://sii.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://toq.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://yar.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://wad.sxryk.cn

[G07] 调用父类方法
来源：http://hdd.aibaodan.cn

Py:   super().greet()
来源：http://ijz.yuanzhike.top

PHP:  parent::greet();
来源：http://vtl.sjlbkw.cn

JS:   super.greet();
来源：http://abd.aibaodan.cn

TS:   super.greet();
来源：http://gmw.hcnkem.com

Java: super.greet();
来源：http://ioc.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dws.zhongyouzk.top

Ruby: super
来源：http://vld.svipenyu.cn

C#:   base.Greet();
来源：http://sis.sufxvd.cn

[G08] 静态方法与属性
来源：http://zsv.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rfp.iojbl.cn

PHP:  public static function f() {}
来源：http://roi.yfazqb.com

JS:   static f() {}
来源：http://cgp.tanke756.top

TS:   static f(): void {}
来源：http://irk.xuanzx.com

Java: static void f() {}
来源：http://tap.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://spc.shzxlz.cn

Ruby: def self.f; end
来源：http://pgl.fengsongda.top

C#:   public static void F() {}
来源：http://zdi.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://psz.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://wga.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://rkh.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jwx.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://hko.sysykeji.top

Java: interface Shape { double area(); }
来源：http://jeu.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://mjb.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hru.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://vxk.cucudq.cn

[G10] 访问控制
来源：http://gry.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://ttk.kuanghao11.cn

PHP:  public / protected / private
来源：http://yyo.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://lvl.shuidangran.top

TS:   public / protected / private
来源：http://owo.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://otn.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://chq.hcnkem.com

Ruby: public / protected / private
来源：http://sgu.daxiang520.top

C#:   public / protected / private / internal
来源：http://smt.fktsv.cn

[G11] getter / setter
来源：http://wro.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://bcx.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://unv.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://joi.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://fnw.yueranfly.top

Java: public String getName() { return name; }
来源：http://lon.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dsh.tian-w.cn

Ruby: attr_accessor :name
来源：http://lyt.xylfe.cn

C#:   public string Name { get; set; }
来源：http://cpc.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://jzt.sweek.top

Py:   def __str__(self): return self.name
来源：http://zjl.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sps.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://sto.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://rid.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://srl.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xrl.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://uud.cheryme.top

C#:   public override string ToString() => Name;
来源：http://zmg.havefunace.top

[G13] 判断对象类型
来源：http://xlw.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://orr.smart0.xyz

PHP:  $u instanceof User
来源：http://icr.chenjidiqi.icu

JS:   u instanceof User
来源：http://ynd.daria6918.cn

TS:   u instanceof User
来源：http://tcm.pycfn.com

Java: u instanceof User
来源：http://nmp.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://baj.yj20258.top

Ruby: u.is_a?(User)
来源：http://jzh.hywenlv.cn

C#:   u is User
来源：http://inm.yj20258.top

[G14] 数据类 / record
来源：http://pus.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ete.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://byb.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qvl.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://clw.epnwcf.com

Java: record User(String name, int age) {}
来源：http://ewo.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://cnc.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eqm.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://xcw.zdbjq.cn

[G15] 枚举
来源：http://ipk.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://osl.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ejp.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pui.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xfn.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://igr.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nae.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://xze.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ted.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://iyk.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pxc.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://oqp.svipenyu.cn

JS:   Object.entries(obj)
来源：http://aox.tanke756.top

TS:   Object.entries(obj)
来源：http://cmn.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwl.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sdm.zdqjudy.top

Ruby: obj.instance_variables
来源：http://gsq.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://zfa.shanyushiyangkeji.top

================================================================================
来源：http://rmh.sysykeji.top

H. 异常与错误处理
来源：http://akc.hammf.cn

================================================================================
来源：http://wyn.haohaochexian.top

[H01] try / catch 基础
来源：http://fsw.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfz.sjlbkw.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whn.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jqc.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppp.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cuk.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mic.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bdg.gotoacloud.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://squ.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://snd.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://ihi.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aao.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nnm.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ice.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://fkp.zdqjudy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xzm.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lig.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rsk.zhijiandao.cn

[H03] 主动抛出异常
来源：http://dur.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://qvm.jinyuanbaomall.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://amc.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://clu.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://vgd.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uee.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zsv.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xio.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dwg.zhengqikj.top

[H04] 自定义异常类型
来源：http://xdp.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://npg.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://otz.bbcook.cn

JS:   class MyError extends Error {}
来源：http://wic.shuidangran.top

TS:   class MyError extends Error {}
来源：http://wkc.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://xim.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eyo.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://bee.sxryk.cn

C#:   class MyException : Exception {}
来源：http://fay.hfpthk.cn

[H05] 捕获特定类型
来源：http://chg.dianchejie.cn

Py:   except ValueError as e:
来源：http://dla.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://awn.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://zge.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://hlv.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://uhy.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cyw.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://wtj.dianchejie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gko.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://qkc.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://brx.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://nmv.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://pkc.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://mst.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bjm.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vrd.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://ece.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://cpg.cashguo.top

[H07] 断言
来源：http://lgz.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://epm.sxryk.cn

PHP:  assert($x > 0);
来源：http://cyk.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://ylj.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://dug.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://tbq.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qul.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://dnt.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://brm.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://dde.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://uzc.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iit.redwolf501.top

JS:   e.message;  e.stack
来源：http://hlx.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://njz.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uru.chenlongwang.top

Go:   err.Error()
来源：http://pmf.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://gwj.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://ivg.vehdjk.com

[H09] 带错误码的异常
来源：http://gts.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ymd.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ljh.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fvp.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lqz.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wre.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwi.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://zkp.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jfg.vehdjk.com

[H10] 资源自动释放
来源：http://xir.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lph.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://adu.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ahr.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bod.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wek.iojbl.cn

Go:   defer f.Close()
来源：http://oab.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sve.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vug.wangdashe.top

================================================================================
来源：http://ldv.quarkkingdee.top

I. 正则表达式
来源：http://kwe.pycfn.com

================================================================================
来源：http://yrb.gogol.net.cn

[I01] 判断是否匹配
来源：http://rkc.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tvk.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://isj.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://ayy.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://dgz.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gkb.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vht.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://xck.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://smg.gotoacloud.top

[I02] 提取所有匹配
来源：http://xpe.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://mkn.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwy.guowangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nuu.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://eco.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xta.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://knw.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://srq.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ybk.ctjpmb.com

[I03] 提取捕获分组
来源：http://fpv.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vxt.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dzj.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yuh.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dzy.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jde.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vyo.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ovh.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wne.dashuyun.cn

[I04] 正则替换
来源：http://duy.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mik.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://unw.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bda.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://nwn.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ftn.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://poy.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ari.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rdb.jyoumei.cn

[I05] 按正则拆分
来源：http://fzx.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iml.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wej.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://lar.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://zdd.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://lpu.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ywu.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://sfa.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hjg.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uat.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ixn.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vie.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppl.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyp.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ilo.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wik.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wus.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yca.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://nhr.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kil.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://due.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tgb.chenjidiqi.icu

TS:   /error/gim
来源：http://obb.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://auj.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://krd.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://bhd.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gbp.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://rek.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mrr.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mal.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlh.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zmh.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://amc.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dad.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tzw.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qqf.tian-w.cn

================================================================================
来源：http://ipb.sjlbkw.cn


<!-- 参考信息 -->