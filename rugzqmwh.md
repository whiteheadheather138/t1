代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://fnt.guowangkeji.top

Ruby: def greet; @name; end
来源：http://fzx.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://xff.yueranfly.top

[G05] 继承
来源：http://xno.xuanzx.com

Py:   class Admin(User): pass
来源：http://zpl.yj20258.top

PHP:  class Admin extends User {}
来源：http://wve.daxiang520.top

JS:   class Admin extends User {}
来源：http://ypz.xuanzx.com

TS:   class Admin extends User {}
来源：http://cqq.sufxvd.cn

Java: class Admin extends User {}
来源：http://uwo.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lac.jinghuilouyu.cn

Ruby: class Admin < User; end
来源：http://hfl.daria6918.cn

C#:   class Admin : User {}
来源：http://yxd.smart0.xyz

[G06] 重写方法
来源：http://lkp.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://xyt.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kww.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://cld.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://rjp.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://zhs.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://swc.guowangkeji.top

Ruby: def greet; "admin"; end
来源：http://lii.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://udw.yj202588.top

[G07] 调用父类方法
来源：http://izj.zhoulong.xyz

Py:   super().greet()
来源：http://gdq.zhixingplan.top

PHP:  parent::greet();
来源：http://nex.cashguo.top

JS:   super.greet();
来源：http://vna.c1oappe.top

TS:   super.greet();
来源：http://bje.xziqi.cn

Java: super.greet();
来源：http://yyh.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://otg.jiagoushi.top

Ruby: super
来源：http://wnp.chenzaomai.com

C#:   base.Greet();
来源：http://iub.yj20258888.top

[G08] 静态方法与属性
来源：http://ptg.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dfk.hammf.cn

PHP:  public static function f() {}
来源：http://jqf.svipenyu.cn

JS:   static f() {}
来源：http://jxp.hnxiangtu.top

TS:   static f(): void {}
来源：http://sxp.yonumen.top

Java: static void f() {}
来源：http://wde.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jnv.pycfn.com

Ruby: def self.f; end
来源：http://fdh.vehdjk.com

C#:   public static void F() {}
来源：http://did.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://ust.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://ppp.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://skv.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oaf.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://fcc.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://pwm.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://vbf.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wjr.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://ysg.cdnleiting.top

[G10] 访问控制
来源：http://fst.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://jkx.shzxlz.cn

PHP:  public / protected / private
来源：http://vtl.guannengcc.top

JS:   #private 字段；其余公开
来源：http://zvk.cdnleiting.top

TS:   public / protected / private
来源：http://zti.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://kwm.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yfa.quarkkingdee.top

Ruby: public / protected / private
来源：http://qqy.ybcxt.top

C#:   public / protected / private / internal
来源：http://xkl.jyoumei.cn

[G11] getter / setter
来源：http://zfl.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://ykv.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://guq.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://tsv.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://rnq.gogol.net.cn

Java: public String getName() { return name; }
来源：http://fag.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://snk.yueranfly.top

Ruby: attr_accessor :name
来源：http://zxf.fengsongda.top

C#:   public string Name { get; set; }
来源：http://dvj.nanxuanxn.top

[G12] 对象转字符串
来源：http://xtm.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://snq.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zwg.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://uku.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://zmv.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://vbr.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bdi.xylfe.cn

Ruby: def to_s; @name; end
来源：http://twa.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://uqa.hesvh.cn

[G13] 判断对象类型
来源：http://eur.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://apf.cdnleiting.top

PHP:  $u instanceof User
来源：http://emi.redwolf501.top

JS:   u instanceof User
来源：http://maw.fanxiaobao.xyz

TS:   u instanceof User
来源：http://ise.yanxiufei.cn

Java: u instanceof User
来源：http://iov.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mbw.guannengcc.top

Ruby: u.is_a?(User)
来源：http://aqv.zhongyouzk.top

C#:   u is User
来源：http://qee.tarul.cn

[G14] 数据类 / record
来源：http://mbv.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kjt.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://asl.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://eht.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://quo.chenjidiqi.icu

Java: record User(String name, int age) {}
来源：http://suy.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://gzd.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://inz.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://nee.zhixingplan.top

[G15] 枚举
来源：http://efz.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcx.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yvz.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tjq.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fwm.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://swv.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bsa.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://wnb.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xyb.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://rgz.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sdq.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://dwp.sysykeji.top

JS:   Object.entries(obj)
来源：http://cec.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://keb.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mxy.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yod.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://wlw.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://dbz.shanyushiyangtech.top

================================================================================
来源：http://pcj.ehwqpu.com

H. 异常与错误处理
来源：http://dfp.zhaomingkeji.xyz

================================================================================
来源：http://zrg.ehwqpu.com

[H01] try / catch 基础
来源：http://zou.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pvw.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qlj.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tlx.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://por.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zhp.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yiu.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ihc.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pzy.hcnkem.com

[H02] finally / ensure 收尾
来源：http://mhe.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://ksv.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nme.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nxo.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vdw.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://lun.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rnt.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zeo.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://njv.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://fuo.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://bcy.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xcy.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://kdu.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://mqb.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://phz.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gwg.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rxn.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://ira.epnwcf.com

[H04] 自定义异常类型
来源：http://pin.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://dri.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://xwf.xinyue.icu

JS:   class MyError extends Error {}
来源：http://dac.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://rpb.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://aui.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mzo.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://zye.yuxming.cn

C#:   class MyException : Exception {}
来源：http://dwq.cdnleiting.top

[H05] 捕获特定类型
来源：http://ujz.zycfv.cn

Py:   except ValueError as e:
来源：http://emd.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kwa.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://zuz.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://zoi.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://lie.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nop.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://yzf.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wqc.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://pbb.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://klr.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dgk.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ktv.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tbs.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqu.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wik.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://cit.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://gxg.iojbl.cn

[H07] 断言
来源：http://nan.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://brl.yonumen.top

PHP:  assert($x > 0);
来源：http://ril.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://aqu.xinyue.icu

TS:   console.assert(x > 0);
来源：http://arn.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://sds.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ads.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mic.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://nss.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://ygz.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://okq.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ert.fengsongda.top

JS:   e.message;  e.stack
来源：http://ivw.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://ywt.guannengcc.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xui.9152youxi.cn

Go:   err.Error()
来源：http://mvg.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://fxe.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://fts.sxryk.cn

[H09] 带错误码的异常
来源：http://psz.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fsv.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mpm.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://duo.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvp.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sux.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vot.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ine.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hws.svipenyu.cn

[H10] 资源自动释放
来源：http://byy.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gsp.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bxj.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qhl.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iuw.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iwc.ydzc1.top

Go:   defer f.Close()
来源：http://xyz.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xvs.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qqf.vehdjk.com

================================================================================
来源：http://jrt.shuidangran.top

I. 正则表达式
来源：http://bzt.feifeiyinyue.top

================================================================================
来源：http://ayh.sjlbkw.cn

[I01] 判断是否匹配
来源：http://bja.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zcb.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://esr.meibo888.top

JS:   /\d+/.test(s)
来源：http://zqy.fzhhl.top

TS:   /\d+/.test(s)
来源：http://stc.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ewq.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ykx.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://bna.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://adl.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://nub.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://kia.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qhw.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fcv.cashguo.top

TS:   s.match(/\d+/g)
来源：http://typ.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lsi.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://grh.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://org.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jzt.sysykeji.top

[I03] 提取捕获分组
来源：http://rta.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hnr.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mnt.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ons.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yfv.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ics.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ojs.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kgb.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ybd.316326.xyz

[I04] 正则替换
来源：http://orn.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pei.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wun.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://cmt.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tmo.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bmf.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lbu.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zuq.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zsp.jqgufenzy.top

[I05] 按正则拆分
来源：http://hwo.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cck.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cfp.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://wlv.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://yje.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://eyd.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hyo.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://yxu.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://twf.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rjn.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://irt.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lti.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsi.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aow.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fvb.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zdb.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tyb.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://peo.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://brp.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zpj.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rzh.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bct.yj20258.top

TS:   /error/gim
来源：http://wub.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dse.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hhf.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://pie.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://utn.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://kfm.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pty.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dru.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yxk.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tzz.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jff.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dyw.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyb.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vxz.jinqigfzy.top

================================================================================
来源：http://vnn.316326.xyz

J. 日期与时间
来源：http://omi.guowangkeji.top

================================================================================
来源：http://bze.yuxming.cn

[J01] 获取当前时间
来源：http://vqh.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wqc.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aod.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://ayf.yj20258888.top

TS:   new Date();  Date.now()
来源：http://fbm.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://izu.fanxiaobao.xyz

Go:   time.Now()
来源：http://ebk.gogol.net.cn

Ruby: Time.now
来源：http://mrj.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://can.fanxiaobao.xyz

[J02] 格式化输出
来源：http://ism.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ljn.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jdc.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wto.c1oappe.top

TS:   d.toISOString()
来源：http://siu.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://owq.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vkf.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbs.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qgy.bjfxy.top


<!-- 参考信息 -->