代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://rrl.birdmap.top

JS:   greet() { return this.name; }
来源：http://zdv.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://yes.ctjpmb.com

Java: String greet() { return name; }
来源：http://ija.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zab.uphjek.com

Ruby: def greet; @name; end
来源：http://pcr.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://qij.mhx1999.top

[G05] 继承
来源：http://nug.haohaochexian.top

Py:   class Admin(User): pass
来源：http://gmy.nwbrower.top

PHP:  class Admin extends User {}
来源：http://cif.dianchejie.cn

JS:   class Admin extends User {}
来源：http://jvx.bbcook.cn

TS:   class Admin extends User {}
来源：http://zqi.gotoacloud.top

Java: class Admin extends User {}
来源：http://ebo.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgx.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://zgc.cqqwz.cn

C#:   class Admin : User {}
来源：http://nrc.ivvv.top

[G06] 重写方法
来源：http://sqo.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://yfk.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nfd.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://hva.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://gzj.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://taf.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oyn.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://sge.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://xli.ydzc1.top

[G07] 调用父类方法
来源：http://eeo.hammf.cn

Py:   super().greet()
来源：http://fhp.chenzaomai.com

PHP:  parent::greet();
来源：http://itm.dashuyun.cn

JS:   super.greet();
来源：http://nrt.vqdsnc.cn

TS:   super.greet();
来源：http://adp.andypj.xyz

Java: super.greet();
来源：http://jrq.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bqw.smart0.xyz

Ruby: super
来源：http://zaa.yfazqb.com

C#:   base.Greet();
来源：http://wob.shuidangran.top

[G08] 静态方法与属性
来源：http://dot.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://htf.jiagoushi.top

PHP:  public static function f() {}
来源：http://qqx.chenjidiqi.icu

JS:   static f() {}
来源：http://rol.hammf.cn

TS:   static f(): void {}
来源：http://eqh.ydzc1.top

Java: static void f() {}
来源：http://ojk.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ahy.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://ams.jinqigfzy.top

C#:   public static void F() {}
来源：http://mdg.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://wof.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://mgj.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mwk.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://usa.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://wix.daria6918.cn

Java: interface Shape { double area(); }
来源：http://krr.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://nrl.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kev.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://ecq.yongpay.top

[G10] 访问控制
来源：http://azv.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://xwx.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://ogh.xinyue.icu

JS:   #private 字段；其余公开
来源：http://icb.jinghuilouyu.cn

TS:   public / protected / private
来源：http://gdy.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://pax.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://swm.guowangkeji.top

Ruby: public / protected / private
来源：http://siz.sysykeji.top

C#:   public / protected / private / internal
来源：http://hcj.jyoumei.cn

[G11] getter / setter
来源：http://fwv.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://txh.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qcq.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://qmk.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://lcg.shzxlz.cn

Java: public String getName() { return name; }
来源：http://zse.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bom.havefunace.top

Ruby: attr_accessor :name
来源：http://mgl.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://bee.hnxiangtu.top

[G12] 对象转字符串
来源：http://axg.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://lvd.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ksv.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://enf.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://ina.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://rvx.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vco.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://jhh.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://xhj.yuanzhike.top

[G13] 判断对象类型
来源：http://jlq.tanke756.top

Py:   isinstance(u, User)
来源：http://dmc.redwolf501.top

PHP:  $u instanceof User
来源：http://cmk.iojbl.cn

JS:   u instanceof User
来源：http://ckr.aizwys.cn

TS:   u instanceof User
来源：http://xze.tanke756.top

Java: u instanceof User
来源：http://mxb.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://myh.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://ujs.zhongyouzk.top

C#:   u is User
来源：http://aqq.c1oappe.top

[G14] 数据类 / record
来源：http://myh.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wkf.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://wgk.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://beh.daria6918.cn

TS:   type User = { name: string; age: number };
来源：http://etx.pycfn.com

Java: record User(String name, int age) {}
来源：http://qst.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://ctk.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://puj.hammf.cn

C#:   record User(string Name, int Age);
来源：http://tnk.fehbvm.com

[G15] 枚举
来源：http://nqb.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://idg.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nav.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dby.yuxming.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ner.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://cag.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://con.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://jsp.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cyx.sweek.top

[G16] 对象转数组 / 字典
来源：http://dos.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wtm.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://dim.jqgfzy.top

JS:   Object.entries(obj)
来源：http://ckq.hysaishi.cn

TS:   Object.entries(obj)
来源：http://rih.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uie.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xox.tianlin.xyz

Ruby: obj.instance_variables
来源：http://hbg.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://hka.52xcode.cn

================================================================================
来源：http://hop.yongpay.top

H. 异常与错误处理
来源：http://deb.yfazqb.com

================================================================================
来源：http://ghi.zhijiandao.cn

[H01] try / catch 基础
来源：http://jji.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bcm.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vqz.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qks.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pxw.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mrq.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cga.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ned.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dqu.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://ujh.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://txt.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qev.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://wrn.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://msc.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://awj.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ljy.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rxw.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eow.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://srq.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://fdd.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xwl.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://cog.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://pdc.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qnp.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zbm.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pde.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://iil.tarul.cn

[H04] 自定义异常类型
来源：http://nll.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://uas.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://khg.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://ixk.sysykeji.top

TS:   class MyError extends Error {}
来源：http://huv.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://clm.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wry.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://yzg.hammf.cn

C#:   class MyException : Exception {}
来源：http://vby.cashguo.top

[H05] 捕获特定类型
来源：http://ixj.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://psn.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hsq.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://tbf.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://hov.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://kpl.jqgufenzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dnt.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://ryz.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vpa.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://dqk.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://yfh.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://bcr.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://zko.cdnleiting.top

TS:   obj?.a?.b;  d ?? default
来源：http://vsg.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qnh.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zgf.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://iog.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://rps.havefunace.top

[H07] 断言
来源：http://hjc.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://ltr.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://tvt.fktsv.cn

JS:   console.assert(x > 0);
来源：http://ndn.bbcook.cn

TS:   console.assert(x > 0);
来源：http://azx.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://ilw.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jcq.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://ogr.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://ucj.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://jae.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://itg.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kmm.ctjpmb.com

JS:   e.message;  e.stack
来源：http://raw.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xkv.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hjy.ctjpmb.com

Go:   err.Error()
来源：http://eic.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://sti.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://tvp.shzxlz.cn

[H09] 带错误码的异常
来源：http://vbc.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lvj.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dog.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ssw.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dtn.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eep.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wnr.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pfc.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mkk.fzhhl.top

[H10] 资源自动释放
来源：http://ifm.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jnz.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wql.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gyp.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yea.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fss.chenlongwang.top

Go:   defer f.Close()
来源：http://pfz.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nys.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vcs.yongpay.top

================================================================================
来源：http://msm.vqdsnc.cn

I. 正则表达式
来源：http://dae.jiagoushi.top

================================================================================
来源：http://eva.zhoulong.xyz

[I01] 判断是否匹配
来源：http://qnm.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wla.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ucg.bjfxy.top

JS:   /\d+/.test(s)
来源：http://ihf.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://kcz.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://htb.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pae.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://ddk.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://buq.yangfankeji.com

[I02] 提取所有匹配
来源：http://ood.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://ibe.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dkk.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nxe.tanke756.top

TS:   s.match(/\d+/g)
来源：http://kbx.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pdi.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dhl.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://dmz.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fbm.jyoumei.cn

[I03] 提取捕获分组
来源：http://qdf.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rdc.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kig.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zzr.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aqz.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jfb.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eoz.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eix.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vwb.bbcook.cn

[I04] 正则替换
来源：http://mvs.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jro.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfr.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://ijg.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bwn.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://wyd.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jkx.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zpm.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jcn.havefunace.top

[I05] 按正则拆分
来源：http://ohk.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dyq.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ihv.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://wwj.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://pab.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://ojb.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gva.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://nbz.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://szl.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oiu.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rkt.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gpw.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqc.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://met.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xac.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxa.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkc.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dve.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://uep.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bbz.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://smi.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jjf.yuxming.cn

TS:   /error/gim
来源：http://lws.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fkp.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tcl.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://ejq.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tgi.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://zrd.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://czx.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fdm.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iwv.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aty.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ofj.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eua.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://flh.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mlz.shangyingyoupin.top

================================================================================
来源：http://xti.gogol.net.cn

J. 日期与时间
来源：http://cuw.guowangkeji.top

================================================================================
来源：http://rdg.zhengqikj.top

[J01] 获取当前时间
来源：http://fzp.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://kbl.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wko.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://mvl.fengsongda.top

TS:   new Date();  Date.now()
来源：http://qml.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fmu.cashguo.top

Go:   time.Now()
来源：http://ewd.gogol.net.cn

Ruby: Time.now
来源：http://iqq.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hcj.zhiwuduotai.top

[J02] 格式化输出
来源：http://prj.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhm.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://law.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qbm.yangfankeji.com

TS:   d.toISOString()
来源：http://vhd.ehwqpu.com


<!-- 参考信息 -->