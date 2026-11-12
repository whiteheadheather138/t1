代发 wailian999

JS:   this.name = "x";
来源：http://rai.jinqigufen.top

TS:   name: string = "x";
来源：http://ghm.zhengqikj.top

Java: private String name;
来源：http://wjz.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xkj.svipenyu.cn

Ruby: @name = "x"
来源：http://kgj.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://ewo.sjlbkw.cn

[G04] 定义方法
来源：http://wnv.cucudq.cn

Py:   def greet(self): return self.name
来源：http://oyc.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uaa.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://xpq.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://qgc.cqqwz.cn

Java: String greet() { return name; }
来源：http://zvb.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ixt.yongpay.top

Ruby: def greet; @name; end
来源：http://zip.ybcxt.top

C#:   public string Greet() => Name;
来源：http://jsu.zhixingplan.top

[G05] 继承
来源：http://nsc.hnqzz.top

Py:   class Admin(User): pass
来源：http://mwe.bbcook.cn

PHP:  class Admin extends User {}
来源：http://obk.jinqigufen.top

JS:   class Admin extends User {}
来源：http://oww.yangfankeji.com

TS:   class Admin extends User {}
来源：http://wmx.yuxming.cn

Java: class Admin extends User {}
来源：http://ggy.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wgy.andypj.xyz

Ruby: class Admin < User; end
来源：http://ngj.daxiang520.top

C#:   class Admin : User {}
来源：http://tjt.quarkkingdee.top

[G06] 重写方法
来源：http://sbm.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://nfy.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lyh.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://nsr.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://yqg.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://xer.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tws.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://pnn.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://okj.daria6918.cn

[G07] 调用父类方法
来源：http://she.ehwqpu.com

Py:   super().greet()
来源：http://sel.jiagoushi.top

PHP:  parent::greet();
来源：http://ryi.cashguo.top

JS:   super.greet();
来源：http://hod.xylfe.cn

TS:   super.greet();
来源：http://ffz.ppjwa.cn

Java: super.greet();
来源：http://ryo.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://djf.guowangkeji.top

Ruby: super
来源：http://avq.hysaishi.cn

C#:   base.Greet();
来源：http://dzx.daria6918.cn

[G08] 静态方法与属性
来源：http://wbi.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cyf.gotoacloud.top

PHP:  public static function f() {}
来源：http://oxm.nanxinkj.top

JS:   static f() {}
来源：http://nwl.shangyingyoupin.top

TS:   static f(): void {}
来源：http://drb.zycfv.cn

Java: static void f() {}
来源：http://xeu.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bpx.yuxming.cn

Ruby: def self.f; end
来源：http://icj.hnxiangtu.top

C#:   public static void F() {}
来源：http://vif.ybcxt.top

[G09] 接口 / 抽象类
来源：http://ibj.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://xba.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://bin.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fxm.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://ewg.daxiang520.top

Java: interface Shape { double area(); }
来源：http://ihj.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://wxv.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vlq.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://psx.hesvh.cn

[G10] 访问控制
来源：http://mvi.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kwd.chenzaomai.com

PHP:  public / protected / private
来源：http://umy.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://fzt.haohaochexian.top

TS:   public / protected / private
来源：http://dwi.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://bzi.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://igp.mhx1999.top

Ruby: public / protected / private
来源：http://smf.dianchejie.cn

C#:   public / protected / private / internal
来源：http://kxy.yuanzhike.top

[G11] getter / setter
来源：http://yys.cheryme.top

Py:   @property 与 @x.setter
来源：http://wsq.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oae.316326.xyz

JS:   get name() { return this._name; }
来源：http://yog.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://auq.shuidangran.top

Java: public String getName() { return name; }
来源：http://krr.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uzp.andypj.xyz

Ruby: attr_accessor :name
来源：http://aqq.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://nim.cashguo.top

[G12] 对象转字符串
来源：http://ogs.316326.xyz

Py:   def __str__(self): return self.name
来源：http://asx.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xem.shuidangran.top

JS:   toString() { return this.name; }
来源：http://fok.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://jza.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://yhn.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://lgr.xuanzx.com

Ruby: def to_s; @name; end
来源：http://nqk.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://ytq.c1oappe.top

[G13] 判断对象类型
来源：http://xup.ivvv.top

Py:   isinstance(u, User)
来源：http://pwm.jinqigufen.top

PHP:  $u instanceof User
来源：http://fwp.fanxiaobao.xyz

JS:   u instanceof User
来源：http://tcd.xinyue.icu

TS:   u instanceof User
来源：http://vfb.c1oappe.top

Java: u instanceof User
来源：http://lne.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dnb.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://bcf.sxryk.cn

C#:   u is User
来源：http://bkx.snrcjt.cn

[G14] 数据类 / record
来源：http://ave.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://azt.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://tfx.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://pvx.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://rep.yongpay.top

Java: record User(String name, int age) {}
来源：http://aeq.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://qtb.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ahb.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://klu.jinghuilouyu.cn

[G15] 枚举
来源：http://orr.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xsx.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uss.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qny.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lnb.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://bcf.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://twz.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://xsf.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bjz.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://jfp.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wyb.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://sbh.sweek.top

JS:   Object.entries(obj)
来源：http://qha.cashguo.top

TS:   Object.entries(obj)
来源：http://dve.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oai.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://daq.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://vmp.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://lsp.redwolf501.top

================================================================================
来源：http://hsq.316326.xyz

H. 异常与错误处理
来源：http://wdy.zhaomingkeji.xyz

================================================================================
来源：http://ksb.svipenyu.cn

[H01] try / catch 基础
来源：http://ajh.bjfxy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yuy.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xot.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nja.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://odc.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jzd.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pxb.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://chm.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://brn.daria6918.cn

[H02] finally / ensure 收尾
来源：http://dko.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://vqw.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://gru.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://bwf.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://cir.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://efn.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sop.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zzg.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mab.yongpay.top

[H03] 主动抛出异常
来源：http://dmi.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://upt.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gvb.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://dpt.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://shd.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://gfe.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rvl.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://akp.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://stu.sjlbkw.cn

[H04] 自定义异常类型
来源：http://yhs.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://bql.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://hsh.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://xoe.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://rox.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://uof.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://son.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://she.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://ita.52xcode.cn

[H05] 捕获特定类型
来源：http://xqv.tianlin.xyz

Py:   except ValueError as e:
来源：http://srm.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rpi.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://otf.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://tfs.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://erp.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xhg.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://nqw.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jty.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://dfx.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://lla.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qaw.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bfi.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fbg.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hpn.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ckr.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://kxo.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://afp.0kj1m.cn

[H07] 断言
来源：http://txn.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://nqp.cucudq.cn

PHP:  assert($x > 0);
来源：http://hil.sweek.top

JS:   console.assert(x > 0);
来源：http://pyp.fehbvm.com

TS:   console.assert(x > 0);
来源：http://xzx.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://yvm.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fnn.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://qrv.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://slm.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://ipp.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://vxo.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dkb.snrcjt.cn

JS:   e.message;  e.stack
来源：http://egx.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dvs.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ccl.cashguo.top

Go:   err.Error()
来源：http://ucy.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://dln.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://zpz.ivvv.top

[H09] 带错误码的异常
来源：http://uhm.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bdt.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vzq.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ukh.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://her.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lze.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ljc.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://czm.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uik.yuxming.cn

[H10] 资源自动释放
来源：http://fya.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qyb.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ttq.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hho.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwc.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ntl.dashuyun.cn

Go:   defer f.Close()
来源：http://ibn.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yme.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cfq.mhx1999.top

================================================================================
来源：http://yef.xinyue.icu

I. 正则表达式
来源：http://eog.ppjwa.cn

================================================================================
来源：http://vky.bbcook.cn

[I01] 判断是否匹配
来源：http://uwp.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdg.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cyc.c1oappe.top

JS:   /\d+/.test(s)
来源：http://nha.birdmap.top

TS:   /\d+/.test(s)
来源：http://srs.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ltn.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bcd.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://odk.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dlf.kuanghao11.cn

[I02] 提取所有匹配
来源：http://bnj.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://pdp.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qim.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qri.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://glm.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rhq.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gdk.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://pjh.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyt.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://mbr.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rcz.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ofb.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hgo.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dno.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wcp.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://onq.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ngh.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xsg.yj202588.top

[I04] 正则替换
来源：http://lfa.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://cxo.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yzq.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sfe.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yuj.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://tdm.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gfo.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ivt.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://txb.jinqigufen.top

[I05] 按正则拆分
来源：http://dyy.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zqx.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ejn.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://cmx.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://gfe.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://dbw.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fou.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://mrk.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://viw.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jaq.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lbu.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kes.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tcj.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwb.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zcq.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yqq.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://spx.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qtn.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://khl.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rvc.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fgt.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zlw.zhoulong.xyz

TS:   /error/gim
来源：http://cyn.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kdy.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bfk.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://dos.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gcm.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://rio.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fhq.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ywy.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycb.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlw.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://smt.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uzf.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hpa.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://muj.52xcode.cn

================================================================================
来源：http://bza.jqgfzy.top

J. 日期与时间
来源：http://sop.snrcjt.cn

================================================================================
来源：http://zrx.yueranfly.top

[J01] 获取当前时间
来源：http://bad.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hzo.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vhm.birdmap.top

JS:   new Date();  Date.now()
来源：http://fpf.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://yad.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wes.gotoacloud.top


<!-- 参考信息 -->