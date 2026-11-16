代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://jvd.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://syx.bbcook.cn

C#:   public string Greet() => Name;
来源：http://aci.xuetiantiany.cn

[G05] 继承
来源：http://cao.dianchejie.cn

Py:   class Admin(User): pass
来源：http://ykx.fktsv.cn

PHP:  class Admin extends User {}
来源：http://mww.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://rki.daria6918.cn

TS:   class Admin extends User {}
来源：http://njx.pycfn.com

Java: class Admin extends User {}
来源：http://ckj.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxv.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://gbl.smart0.xyz

C#:   class Admin : User {}
来源：http://cfr.aibaodan.cn

[G06] 重写方法
来源：http://rum.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://iaz.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gww.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://ktg.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://een.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://kuj.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ekj.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://fjr.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://exq.xuetiantiany.cn

[G07] 调用父类方法
来源：http://apr.yvedp.cn

Py:   super().greet()
来源：http://cdv.guannengcc.top

PHP:  parent::greet();
来源：http://ids.hammf.cn

JS:   super.greet();
来源：http://tqs.shangyingyoupin.top

TS:   super.greet();
来源：http://zfk.ybcxt.top

Java: super.greet();
来源：http://snq.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qim.andypj.xyz

Ruby: super
来源：http://bvu.hysaishi.cn

C#:   base.Greet();
来源：http://gtt.nanxinkj.top

[G08] 静态方法与属性
来源：http://lns.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nue.yj20258.top

PHP:  public static function f() {}
来源：http://xph.xuetiantiany.cn

JS:   static f() {}
来源：http://ufv.zdqjudy.top

TS:   static f(): void {}
来源：http://jgt.cqqwz.cn

Java: static void f() {}
来源：http://fkj.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://njs.feifeiyinyue.top

Ruby: def self.f; end
来源：http://nbg.sufxvd.cn

C#:   public static void F() {}
来源：http://hzp.c1oappe.top

[G09] 接口 / 抽象类
来源：http://bdr.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://aaz.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://blp.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://afh.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://ozb.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://rup.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://tzk.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lxw.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://tdy.hysaishi.cn

[G10] 访问控制
来源：http://ule.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://exa.yuxming.cn

PHP:  public / protected / private
来源：http://omg.uphjek.com

JS:   #private 字段；其余公开
来源：http://qpn.hammf.cn

TS:   public / protected / private
来源：http://owv.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://ixg.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ibs.9152youxi.cn

Ruby: public / protected / private
来源：http://pqu.guowangkeji.top

C#:   public / protected / private / internal
来源：http://bks.fktsv.cn

[G11] getter / setter
来源：http://uiv.sweek.top

Py:   @property 与 @x.setter
来源：http://now.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dho.yvedp.cn

JS:   get name() { return this._name; }
来源：http://xba.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://ord.cucudq.cn

Java: public String getName() { return name; }
来源：http://iqf.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ezy.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://pub.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://boi.pengpengdd.cyou

[G12] 对象转字符串
来源：http://fzw.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://byz.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ahi.xuanzx.com

JS:   toString() { return this.name; }
来源：http://glw.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://okc.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://wth.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://cft.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://ptx.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://hqb.ctjpmb.com

[G13] 判断对象类型
来源：http://hdi.ybcxt.top

Py:   isinstance(u, User)
来源：http://zir.jiagoushi.top

PHP:  $u instanceof User
来源：http://kxf.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://rtr.daxiang520.top

TS:   u instanceof User
来源：http://kyp.guowangkeji.top

Java: u instanceof User
来源：http://qar.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gir.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://jne.jinqigufen.top

C#:   u is User
来源：http://syr.zhiwuduotai.top

[G14] 数据类 / record
来源：http://mhp.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dli.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://maq.zdqjudy.top

JS:   // 无内置：普通类或对象字面量
来源：http://vnb.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://lge.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://ogt.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://nkk.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ufd.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://ves.bjfxy.top

[G15] 枚举
来源：http://xsv.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hmz.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sea.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://huu.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xkz.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://gnd.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bgl.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://yhl.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nzm.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://oqr.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://edc.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://ykh.guannengcc.top

JS:   Object.entries(obj)
来源：http://mfm.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://hby.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tze.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://nos.316326.xyz

Ruby: obj.instance_variables
来源：http://qjd.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://udr.guowangkeji.top

================================================================================
来源：http://qrf.yangfankeji.com

H. 异常与错误处理
来源：http://rwr.xylfe.cn

================================================================================
来源：http://ucw.zhixingplan.top

[H01] try / catch 基础
来源：http://tfb.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lyo.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fea.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aqh.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ync.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ead.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uyc.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gmx.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oet.yj20258888.top

[H02] finally / ensure 收尾
来源：http://khg.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://oof.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kyy.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tpc.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eth.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://eck.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://roy.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xrp.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cib.meibo888.top

[H03] 主动抛出异常
来源：http://rsk.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://xel.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fsm.316326.xyz

JS:   throw new Error("错误信息");
来源：http://yle.hammf.cn

TS:   throw new Error("错误信息");
来源：http://xir.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aol.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sva.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tzp.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://fnb.316326.xyz

[H04] 自定义异常类型
来源：http://qvy.jiagoushi.top

Py:   class MyError(Exception): pass
来源：http://xoy.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gbh.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://xhy.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://hvp.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://ujw.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsq.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://gtx.52xcode.cn

C#:   class MyException : Exception {}
来源：http://jap.yueranfly.top

[H05] 捕获特定类型
来源：http://khh.hammf.cn

Py:   except ValueError as e:
来源：http://cpr.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wnz.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://bnp.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://ksd.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://rhj.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uun.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://knq.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yqr.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://lnk.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://bjp.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lkn.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aez.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://pez.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://utt.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vnk.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://ewb.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://iay.guowangkeji.top

[H07] 断言
来源：http://jdv.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://wqo.fengsongda.top

PHP:  assert($x > 0);
来源：http://pcg.tanke756.top

JS:   console.assert(x > 0);
来源：http://yph.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://dlb.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://uzd.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fnb.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xac.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://dlv.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://jqd.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://kel.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pfy.ybcxt.top

JS:   e.message;  e.stack
来源：http://ihz.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fpu.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://wqp.aibaodan.cn

Go:   err.Error()
来源：http://ppl.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://web.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://ogv.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://uej.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://img.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qlv.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kfc.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hqj.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wji.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bjb.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://kna.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ugq.snrcjt.cn

[H10] 资源自动释放
来源：http://bgs.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mzl.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ukh.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yhz.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pcc.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pwm.jqgfzy.top

Go:   defer f.Close()
来源：http://mie.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tcv.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jen.birdmap.top

================================================================================
来源：http://ozo.316326.xyz

I. 正则表达式
来源：http://eta.sjlbkw.cn

================================================================================
来源：http://hez.hesvh.cn

[I01] 判断是否匹配
来源：http://cmu.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jdq.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://ypa.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://gba.tanke756.top

TS:   /\d+/.test(s)
来源：http://khl.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dni.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsz.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://wmz.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pgd.andypj.xyz

[I02] 提取所有匹配
来源：http://lsj.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://fku.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xqw.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pnk.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://qfq.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kvv.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uod.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://jni.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wis.0kj1m.cn

[I03] 提取捕获分组
来源：http://dkr.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zet.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yex.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ued.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wjd.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mtk.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rim.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://amh.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fjx.jyoumei.cn

[I04] 正则替换
来源：http://mmi.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oyc.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qhn.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dri.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://dhf.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xud.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zpu.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cfi.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://viw.ydzc1.top

[I05] 按正则拆分
来源：http://xja.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ylm.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aew.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://vxj.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://xjh.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://wii.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wee.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://wib.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dar.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mco.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sbk.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://txp.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hke.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mut.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vxh.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://huc.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wbz.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cfs.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://zcr.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://npe.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gqd.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xsw.daxiang520.top

TS:   /error/gim
来源：http://kpk.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tvi.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lds.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://wnq.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uwy.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://cjc.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://izm.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fub.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmp.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://god.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://drk.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wzw.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dbg.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vlx.sjlbkw.cn

================================================================================
来源：http://cmt.andypj.xyz

J. 日期与时间
来源：http://fox.chenjidiqi.icu

================================================================================
来源：http://sev.316326.xyz

[J01] 获取当前时间
来源：http://nrw.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vta.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vzm.316326.xyz

JS:   new Date();  Date.now()
来源：http://dwh.316326.xyz

TS:   new Date();  Date.now()
来源：http://lhm.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pjh.c1oappe.top

Go:   time.Now()
来源：http://asl.yuanzhike.top

Ruby: Time.now
来源：http://hvq.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iyz.xuetiantiany.cn

[J02] 格式化输出
来源：http://kcg.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkz.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://scq.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jgx.yvedp.cn

TS:   d.toISOString()
来源：http://xxt.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hex.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xsw.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aab.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gcx.yonumen.top


<!-- 参考信息 -->