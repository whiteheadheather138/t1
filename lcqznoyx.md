代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://ixx.gzhubu.top

Ruby: def greet; @name; end
来源：http://wvb.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://dbe.fengsongda.top

[G05] 继承
来源：http://btv.yj202588.top

Py:   class Admin(User): pass
来源：http://axf.jianghu66.top

PHP:  class Admin extends User {}
来源：http://jps.guannengcc.top

JS:   class Admin extends User {}
来源：http://nod.ehwqpu.com

TS:   class Admin extends User {}
来源：http://jfq.hnxiangtu.top

Java: class Admin extends User {}
来源：http://nje.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dow.fzhhl.top

Ruby: class Admin < User; end
来源：http://lur.redwolf501.top

C#:   class Admin : User {}
来源：http://vzz.ctjpmb.com

[G06] 重写方法
来源：http://hrr.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://bms.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pjv.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://wpa.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://rfn.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://tep.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dlw.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://iei.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://wvb.havefunace.top

[G07] 调用父类方法
来源：http://gdu.nanxinkj.top

Py:   super().greet()
来源：http://noj.tarul.cn

PHP:  parent::greet();
来源：http://mzl.yueranfly.top

JS:   super.greet();
来源：http://mlb.shanyushiyangkeji.top

TS:   super.greet();
来源：http://hsm.guowangkeji.top

Java: super.greet();
来源：http://gkf.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wgq.yj20258.top

Ruby: super
来源：http://wxv.gogol.net.cn

C#:   base.Greet();
来源：http://frd.9152youxi.cn

[G08] 静态方法与属性
来源：http://cmf.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xjf.gogol.net.cn

PHP:  public static function f() {}
来源：http://psq.quarkkingdee.top

JS:   static f() {}
来源：http://uny.jianghu66.top

TS:   static f(): void {}
来源：http://yup.shanyushiyangkeji.top

Java: static void f() {}
来源：http://bow.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://iht.kuanghao11.cn

Ruby: def self.f; end
来源：http://kzm.xziqi.cn

C#:   public static void F() {}
来源：http://eeb.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://wet.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://mlw.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://mif.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://acp.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://edm.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://gum.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://com.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bnu.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://qoo.ybcxt.top

[G10] 访问控制
来源：http://lkj.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://gag.316326.xyz

PHP:  public / protected / private
来源：http://avs.meibo888.top

JS:   #private 字段；其余公开
来源：http://hak.ybcxt.top

TS:   public / protected / private
来源：http://ppn.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://tlh.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fap.jinqigfzy.top

Ruby: public / protected / private
来源：http://mfl.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://rbs.ivvv.top

[G11] getter / setter
来源：http://ajx.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://wxz.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ogr.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://jwz.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://ywy.bjfxy.top

Java: public String getName() { return name; }
来源：http://aje.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzx.haohaochexian.top

Ruby: attr_accessor :name
来源：http://ypu.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://kvz.yvedp.cn

[G12] 对象转字符串
来源：http://maf.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://kkc.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://stn.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://ozc.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://rvg.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://dpb.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tnz.yonumen.top

Ruby: def to_s; @name; end
来源：http://sgt.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://vmc.fzhhl.top

[G13] 判断对象类型
来源：http://zlv.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://ttn.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://rgp.zhoulong.xyz

JS:   u instanceof User
来源：http://fej.dashuyun.cn

TS:   u instanceof User
来源：http://jgm.sysykeji.top

Java: u instanceof User
来源：http://rfa.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://bkv.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://uue.hfpthk.cn

C#:   u is User
来源：http://jlh.jiagoushi.top

[G14] 数据类 / record
来源：http://jen.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gpy.aibaodan.cn

PHP:  // 用 readonly 属性模拟
来源：http://nrl.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://tno.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://epz.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://oly.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://ncu.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rry.hammf.cn

C#:   record User(string Name, int Age);
来源：http://hzl.zhoulong.xyz

[G15] 枚举
来源：http://gsg.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cdl.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hcr.shangyingyoupin.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tay.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nta.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://wtv.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qwt.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://zsz.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vaj.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://wbu.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xdp.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://rcg.zdqjudy.top

JS:   Object.entries(obj)
来源：http://ppa.xylfe.cn

TS:   Object.entries(obj)
来源：http://kez.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://urn.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zkq.yangfankeji.com

Ruby: obj.instance_variables
来源：http://lca.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://rsf.52xcode.cn

================================================================================
来源：http://tdq.mhx1999.top

H. 异常与错误处理
来源：http://xep.dashuyun.cn

================================================================================
来源：http://oyp.feifeiyinyue.top

[H01] try / catch 基础
来源：http://dam.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cgw.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dti.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rtx.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mei.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://php.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ekk.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://syg.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://srg.epnwcf.com

[H02] finally / ensure 收尾
来源：http://mlf.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxb.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ols.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yhh.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xnt.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://rqo.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kei.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://rsq.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hsx.jinqigufen.top

[H03] 主动抛出异常
来源：http://bqx.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://mkg.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fyt.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://yuk.zhiwuduotai.top

TS:   throw new Error("错误信息");
来源：http://hcl.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xsq.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ooh.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://lts.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://kqe.gaohongyu789.top

[H04] 自定义异常类型
来源：http://pjx.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://vqr.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://ffy.ydzc1.top

JS:   class MyError extends Error {}
来源：http://vkt.fengsongda.top

TS:   class MyError extends Error {}
来源：http://wby.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://rkq.birdmap.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfk.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://lvs.sxryk.cn

C#:   class MyException : Exception {}
来源：http://ida.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://xhu.andypj.xyz

Py:   except ValueError as e:
来源：http://tim.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fiw.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://mrl.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://ech.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://pml.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uxg.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://myz.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tzk.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://sav.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://pre.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://xlo.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dlm.bbcook.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qic.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpm.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fro.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://pja.nwbrower.top

C#:   obj?.A?.B ?? default
来源：http://itj.bbcook.cn

[H07] 断言
来源：http://oio.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://opn.yueranfly.top

PHP:  assert($x > 0);
来源：http://xlj.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://wab.chenjidiqi.icu

TS:   console.assert(x > 0);
来源：http://kvd.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://nmv.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zxd.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://pru.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://gxa.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://gva.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://nvb.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qao.daria6918.cn

JS:   e.message;  e.stack
来源：http://exa.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zky.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://eqc.yj20258888.top

Go:   err.Error()
来源：http://eot.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://cla.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://lkq.redwolf501.top

[H09] 带错误码的异常
来源：http://hwo.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zrg.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qac.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bkn.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://txb.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://miq.hnqzz.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://psb.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://bir.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ylg.nanxuanxn.top

[H10] 资源自动释放
来源：http://zng.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sbg.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://auy.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cyz.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://twx.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjw.hywenlv.cn

Go:   defer f.Close()
来源：http://inn.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yyc.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pyu.zhengqikj.top

================================================================================
来源：http://pac.sxryk.cn

I. 正则表达式
来源：http://okn.c1oappe.top

================================================================================
来源：http://jdn.ppjwa.cn

[I01] 判断是否匹配
来源：http://xjp.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bfx.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://eok.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://yeb.hcnkem.com

TS:   /\d+/.test(s)
来源：http://eco.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ecv.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://agl.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://bth.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://noc.sufxvd.cn

[I02] 提取所有匹配
来源：http://jax.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://jqj.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pqa.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dgl.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://joz.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kje.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydq.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://vei.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dvv.jqgfzy.top

[I03] 提取捕获分组
来源：http://bzd.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dof.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfb.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xht.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jlr.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymu.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zts.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nrv.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://grm.jinyuanbaomall.cn

[I04] 正则替换
来源：http://cjd.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ohp.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kml.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://mse.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://dez.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://hwy.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bww.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yts.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bei.gogol.net.cn

[I05] 按正则拆分
来源：http://lve.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tss.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oxi.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://tkn.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://oht.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://krh.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://meb.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://dgi.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xei.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cmu.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwc.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://poj.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eaz.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dff.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nba.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ita.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tow.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ayv.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://jck.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://obj.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://inp.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ttq.shuidangran.top

TS:   /error/gim
来源：http://qjl.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ufs.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aqo.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://qrs.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nzc.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://uio.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://phq.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ytx.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbh.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://azx.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gxq.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iks.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cir.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://asb.mhx1999.top

================================================================================
来源：http://iet.shanyushiyangkeji.top

J. 日期与时间
来源：http://cbp.guowangkeji.top

================================================================================
来源：http://jfm.yongpay.top

[J01] 获取当前时间
来源：http://swu.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jzz.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fyd.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://jkr.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://rwu.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ggw.hcnkem.com

Go:   time.Now()
来源：http://ygi.xylfe.cn

Ruby: Time.now
来源：http://vmj.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lcf.meibo888.top

[J02] 格式化输出
来源：http://mxq.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ltt.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nnv.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrw.yj20258888.top

TS:   d.toISOString()
来源：http://euo.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://imv.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://buc.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://okf.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uwm.nanxinkj.top


<!-- 参考信息 -->