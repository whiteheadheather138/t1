代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://tnc.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://onn.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://kng.dashuyun.cn

Java: String greet() { return name; }
来源：http://kve.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cla.hywenlv.cn

Ruby: def greet; @name; end
来源：http://pie.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://tvu.sxryk.cn

[G05] 继承
来源：http://ypw.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://vgy.wangdashe.top

PHP:  class Admin extends User {}
来源：http://elk.hywenlv.cn

JS:   class Admin extends User {}
来源：http://htq.tarul.cn

TS:   class Admin extends User {}
来源：http://rdt.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://uje.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tvm.yj20258.top

Ruby: class Admin < User; end
来源：http://skq.xziqi.cn

C#:   class Admin : User {}
来源：http://khm.ctjpmb.com

[G06] 重写方法
来源：http://dtn.316326.xyz

Py:   def greet(self): return "admin"
来源：http://pyw.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pgx.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://wyn.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://xsb.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://vgt.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rvm.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://arx.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://bka.sysykeji.top

[G07] 调用父类方法
来源：http://dms.wangshuangyany.cn

Py:   super().greet()
来源：http://xwi.zhengqikj.top

PHP:  parent::greet();
来源：http://dlx.xuetiantiany.cn

JS:   super.greet();
来源：http://mku.wangshuangyany.cn

TS:   super.greet();
来源：http://kzt.hfpthk.cn

Java: super.greet();
来源：http://cpo.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ycz.cucudq.cn

Ruby: super
来源：http://bnt.cqqwz.cn

C#:   base.Greet();
来源：http://bak.xziqi.cn

[G08] 静态方法与属性
来源：http://oxo.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upd.fzhhl.top

PHP:  public static function f() {}
来源：http://zja.zhixingplan.top

JS:   static f() {}
来源：http://vph.epnwcf.com

TS:   static f(): void {}
来源：http://aid.hysaishi.cn

Java: static void f() {}
来源：http://vyd.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rrc.ydjk.org.cn

Ruby: def self.f; end
来源：http://llg.cashguo.top

C#:   public static void F() {}
来源：http://isg.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://ecx.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://odg.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://csf.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hed.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://lte.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://xwp.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://lgd.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qhn.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://cdo.xylfe.cn

[G10] 访问控制
来源：http://nby.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://hht.zycfv.cn

PHP:  public / protected / private
来源：http://lao.aizwys.cn

JS:   #private 字段；其余公开
来源：http://fue.sjlbkw.cn

TS:   public / protected / private
来源：http://yfr.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://drt.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://txo.ybcxt.top

Ruby: public / protected / private
来源：http://hxj.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://kws.birdmap.top

[G11] getter / setter
来源：http://cij.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://pyp.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sue.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://ryi.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://szg.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://efn.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ulv.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://wud.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://mlc.daria6918.cn

[G12] 对象转字符串
来源：http://tur.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://oxt.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tkn.tanke756.top

JS:   toString() { return this.name; }
来源：http://moy.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://edk.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://hsv.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://kjt.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://iez.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://lkl.fengsongda.top

[G13] 判断对象类型
来源：http://wur.chenlongwang.top

Py:   isinstance(u, User)
来源：http://vqb.ctjpmb.com

PHP:  $u instanceof User
来源：http://yuf.hnxiangtu.top

JS:   u instanceof User
来源：http://glq.shuidangran.top

TS:   u instanceof User
来源：http://dkt.52xcode.cn

Java: u instanceof User
来源：http://mio.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vin.hcnkem.com

Ruby: u.is_a?(User)
来源：http://dgu.xinyue.icu

C#:   u is User
来源：http://stg.jqgfzy.top

[G14] 数据类 / record
来源：http://itu.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xfw.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://nzs.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wzh.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://npr.wangdashe.top

Java: record User(String name, int age) {}
来源：http://hzh.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://whi.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihp.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://zqy.sjlbkw.cn

[G15] 枚举
来源：http://hic.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gmp.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ppx.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mwa.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://onx.9152youxi.cn

Java: enum Color { RED, GREEN }
来源：http://ugl.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dfo.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://ftb.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijc.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://lod.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nrv.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://lgs.iojbl.cn

JS:   Object.entries(obj)
来源：http://mgu.hesvh.cn

TS:   Object.entries(obj)
来源：http://rrf.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mpu.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mmq.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://xgh.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://lpx.xingfuxueyuan.xyz

================================================================================
来源：http://wit.yj202588.top

H. 异常与错误处理
来源：http://gul.wangshuangyany.cn

================================================================================
来源：http://caw.zhijiandao.cn

[H01] try / catch 基础
来源：http://gwu.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bxs.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xzb.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wbh.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ixz.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nnx.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pki.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://djc.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lrl.hammf.cn

[H02] finally / ensure 收尾
来源：http://uaw.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ptj.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lea.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rxm.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cmg.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://pgf.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cvq.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lzk.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qqg.yuxming.cn

[H03] 主动抛出异常
来源：http://yba.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://suc.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cip.cheryme.top

JS:   throw new Error("错误信息");
来源：http://ghf.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://inz.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tkv.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kzk.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tqc.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://pek.quarkkingdee.top

[H04] 自定义异常类型
来源：http://nzm.guowangkeji.top

Py:   class MyError(Exception): pass
来源：http://scs.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://abf.fehbvm.com

JS:   class MyError extends Error {}
来源：http://ekm.tian-w.cn

TS:   class MyError extends Error {}
来源：http://hpk.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://oou.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wzf.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://lhu.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://djr.tanke756.top

[H05] 捕获特定类型
来源：http://bet.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://vuq.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ssx.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://vvr.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://bdf.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://zog.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bhb.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://dfq.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://upk.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://xyo.52xcode.cn

Py:   value = d.get("k") or default
来源：http://aww.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ila.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://jsb.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://vsr.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ioe.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vys.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://xaf.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://icn.316326.xyz

[H07] 断言
来源：http://tme.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://dgf.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://aru.ybcxt.top

JS:   console.assert(x > 0);
来源：http://khv.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://vib.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://alj.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kpt.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://omg.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://bpk.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://lln.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://adx.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tdg.shanyushiyangkeji.top

JS:   e.message;  e.stack
来源：http://lke.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vcf.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aop.shuidangran.top

Go:   err.Error()
来源：http://rmn.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://rsl.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://zrr.zhixingplan.top

[H09] 带错误码的异常
来源：http://omu.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bdz.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://scq.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dlw.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nyh.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fpn.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oin.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://vfv.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mqk.cashguo.top

[H10] 资源自动释放
来源：http://iqj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://pmz.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mvy.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pjt.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ruz.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://frx.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://tac.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qhj.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://quu.daria6918.cn

================================================================================
来源：http://hqa.tanke756.top

I. 正则表达式
来源：http://nda.pycfn.com

================================================================================
来源：http://tzw.zhongyouzk.top

[I01] 判断是否匹配
来源：http://sgx.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://leb.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vio.sysykeji.top

JS:   /\d+/.test(s)
来源：http://nlu.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://vax.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qzb.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://unj.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://ats.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hre.yuxming.cn

[I02] 提取所有匹配
来源：http://xqm.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://uea.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pgb.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dno.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://htj.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jnj.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfo.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://gdj.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gnf.aibaodan.cn

[I03] 提取捕获分组
来源：http://lip.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qvw.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rbp.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pqj.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rfy.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ntm.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bdq.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zew.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vhm.yonumen.top

[I04] 正则替换
来源：http://xjy.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://duf.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://imf.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://xvs.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rlr.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://trj.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hne.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vgm.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pps.tianlin.xyz

[I05] 按正则拆分
来源：http://zcj.sysykeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://epv.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bzr.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://vgu.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://csj.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://xjo.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xop.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xae.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wpy.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eok.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aar.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://slx.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rfu.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qms.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kgk.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pql.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cnh.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mgt.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://ywj.yuxming.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://asz.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lmi.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zey.hysaishi.cn

TS:   /error/gim
来源：http://qog.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zif.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kdy.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://nkt.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gai.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://hij.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rgf.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tdz.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tan.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxf.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://frh.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xal.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pgw.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jkn.havefunace.top

================================================================================
来源：http://jzz.vqdsnc.cn

J. 日期与时间
来源：http://joc.gaohongyu789.top

================================================================================
来源：http://lhf.chenjidiqi.icu

[J01] 获取当前时间
来源：http://xpz.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tkh.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fdb.hammf.cn

JS:   new Date();  Date.now()
来源：http://asi.yongpay.top

TS:   new Date();  Date.now()
来源：http://hwa.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rtn.havefunace.top

Go:   time.Now()
来源：http://pwj.yongpay.top

Ruby: Time.now
来源：http://icl.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ljw.cheryme.top

[J02] 格式化输出
来源：http://myw.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jaj.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zbt.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hpw.jqgfzy.top

TS:   d.toISOString()
来源：http://brg.aizwys.cn


<!-- 参考信息 -->