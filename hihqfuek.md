代发 wailian999

[G06] 重写方法
来源：http://ugw.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://suf.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tlu.birdmap.top

JS:   greet() { return "admin"; }
来源：http://wmj.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://vwm.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wmq.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tys.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://vbm.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://pyw.jqgfzy.top

[G07] 调用父类方法
来源：http://nvf.bjfxy.top

Py:   super().greet()
来源：http://pqv.aizwys.cn

PHP:  parent::greet();
来源：http://evh.guowangkeji.top

JS:   super.greet();
来源：http://ypj.bjfxy.top

TS:   super.greet();
来源：http://czm.aizwys.cn

Java: super.greet();
来源：http://cso.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ngt.hesvh.cn

Ruby: super
来源：http://ctz.feifeiyinyue.top

C#:   base.Greet();
来源：http://cxh.nwbrower.top

[G08] 静态方法与属性
来源：http://uso.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rhm.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://rfr.shuidangran.top

JS:   static f() {}
来源：http://sbq.wangshuangyany.cn

TS:   static f(): void {}
来源：http://gnv.xinyue.icu

Java: static void f() {}
来源：http://fag.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dmr.cheryme.top

Ruby: def self.f; end
来源：http://hql.sjlbkw.cn

C#:   public static void F() {}
来源：http://vlu.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://ocl.zhoulong.xyz

Py:   from abc import ABC, abstractmethod
来源：http://vxs.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://tbh.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://pvg.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://vom.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://yzz.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://gqs.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://anb.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://vro.snrcjt.cn

[G10] 访问控制
来源：http://xsu.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://guc.sjlbkw.cn

PHP:  public / protected / private
来源：http://riv.ybcxt.top

JS:   #private 字段；其余公开
来源：http://wfy.xylfe.cn

TS:   public / protected / private
来源：http://zrj.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://ddh.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://upr.yangfankeji.com

Ruby: public / protected / private
来源：http://ghr.daria6918.cn

C#:   public / protected / private / internal
来源：http://het.havefunace.top

[G11] getter / setter
来源：http://zlo.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://lvw.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zdt.c1oappe.top

JS:   get name() { return this._name; }
来源：http://brn.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://svu.hnqzz.top

Java: public String getName() { return name; }
来源：http://wtd.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zwj.guowangkeji.top

Ruby: attr_accessor :name
来源：http://fgl.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://irj.fengsongda.top

[G12] 对象转字符串
来源：http://wga.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://yck.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xmq.jianghu66.top

JS:   toString() { return this.name; }
来源：http://qzz.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://xly.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://vuz.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iwq.yj20258888.top

Ruby: def to_s; @name; end
来源：http://xkx.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://isc.daria6918.cn

[G13] 判断对象类型
来源：http://scv.tanke756.top

Py:   isinstance(u, User)
来源：http://nbf.zhijiandao.cn

PHP:  $u instanceof User
来源：http://ble.sxryk.cn

JS:   u instanceof User
来源：http://wba.shuidangran.top

TS:   u instanceof User
来源：http://yfa.sweek.top

Java: u instanceof User
来源：http://guv.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ahg.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://ggo.feifeiyinyue.top

C#:   u is User
来源：http://kbx.zdbjq.cn

[G14] 数据类 / record
来源：http://erj.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lbq.cheryme.top

PHP:  // 用 readonly 属性模拟
来源：http://bzz.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://cxg.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://ryk.smart0.xyz

Java: record User(String name, int age) {}
来源：http://nec.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://vlv.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwz.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://ici.dashuyun.cn

[G15] 枚举
来源：http://usa.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fmx.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vul.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nhs.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vuu.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://kzd.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ygj.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://eaf.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pwz.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://uow.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kmj.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://vxf.jqgfzy.top

JS:   Object.entries(obj)
来源：http://kff.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://amv.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qop.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://fyf.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://qzb.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://nqi.bjfxy.top

================================================================================
来源：http://mea.redwolf501.top

H. 异常与错误处理
来源：http://xmc.xuanzx.com

================================================================================
来源：http://ool.bjfxy.top

[H01] try / catch 基础
来源：http://kec.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://spv.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xjp.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nlx.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xhf.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pzg.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xdq.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://omx.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aod.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://bcm.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lzi.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ghl.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://veq.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bwi.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://utf.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aqt.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qzg.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mtq.yj20258888.top

[H03] 主动抛出异常
来源：http://lye.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://mxe.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nat.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://vcs.daxiang520.top

TS:   throw new Error("错误信息");
来源：http://nxk.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hoz.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tls.hongshengwenyu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xve.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://vnh.andypj.xyz

[H04] 自定义异常类型
来源：http://edt.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://xtd.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mmi.smart0.xyz

JS:   class MyError extends Error {}
来源：http://isu.daxiang520.top

TS:   class MyError extends Error {}
来源：http://qaf.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://lts.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://muo.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://rkb.birdmap.top

C#:   class MyException : Exception {}
来源：http://dkp.guannengcc.top

[H05] 捕获特定类型
来源：http://zkd.pycfn.com

Py:   except ValueError as e:
来源：http://lyr.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mhx.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ntp.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://tgm.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://wnl.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pik.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://gda.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lad.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://zuf.birdmap.top

Py:   value = d.get("k") or default
来源：http://fen.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://isb.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nfy.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ktf.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://okp.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sxn.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://zjc.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://azo.nanxuanxn.top

[H07] 断言
来源：http://ett.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://irp.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://wkk.yj20258888.top

JS:   console.assert(x > 0);
来源：http://qye.meibo888.top

TS:   console.assert(x > 0);
来源：http://ahu.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://sph.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ace.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://nka.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://znq.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://oou.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://luc.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zze.hesvh.cn

JS:   e.message;  e.stack
来源：http://rfx.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iso.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zfo.tarul.cn

Go:   err.Error()
来源：http://pvp.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://ujs.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://owd.shuidangran.top

[H09] 带错误码的异常
来源：http://svy.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eei.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wll.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tbn.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dxs.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zpb.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qyz.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://npe.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wai.dashuyun.cn

[H10] 资源自动释放
来源：http://mge.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://slp.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ojm.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mgy.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rxi.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://obt.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://nmm.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dbe.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tyo.hfpthk.cn

================================================================================
来源：http://inq.gaohongyu789.top

I. 正则表达式
来源：http://cil.aibaodan.cn

================================================================================
来源：http://fjo.yuxming.cn

[I01] 判断是否匹配
来源：http://ifi.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sfw.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jrd.ydzc1.top

JS:   /\d+/.test(s)
来源：http://vkl.vehdjk.com

TS:   /\d+/.test(s)
来源：http://gar.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eau.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ehu.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://amh.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hke.cashguo.top

[I02] 提取所有匹配
来源：http://rba.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://agh.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yov.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cmb.316326.xyz

TS:   s.match(/\d+/g)
来源：http://ybc.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mpz.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qpg.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://kwe.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oda.fengsongda.top

[I03] 提取捕获分组
来源：http://aiy.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pnr.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vde.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ewk.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pcu.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apm.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hcw.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uye.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lhp.kuanghao11.cn

[I04] 正则替换
来源：http://xoe.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ewe.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rsz.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ije.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://ooa.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://dzb.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://phy.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yxa.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rpe.xylfe.cn

[I05] 按正则拆分
来源：http://ujg.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jrt.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://itg.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://hvf.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://rzh.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://zsm.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://avf.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://wzh.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vco.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vjc.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zly.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wye.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvo.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://grr.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cca.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://etg.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bmq.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jec.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://wwu.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cvg.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ews.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ums.zhijiandao.cn

TS:   /error/gim
来源：http://ima.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bsc.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://txz.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://nma.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://umw.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://ktm.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mbr.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kgz.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nvh.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hcf.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://nbu.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gls.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pvb.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ngk.hnxiangtu.top

================================================================================
来源：http://vcl.jinqigfzy.top

J. 日期与时间
来源：http://rbm.wangshuangyany.cn

================================================================================
来源：http://smo.zdbjq.cn

[J01] 获取当前时间
来源：http://can.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mrk.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rcz.ybcxt.top

JS:   new Date();  Date.now()
来源：http://jmv.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://jfy.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ome.nanxuanxn.top

Go:   time.Now()
来源：http://qmz.uphjek.com

Ruby: Time.now
来源：http://zjn.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bez.feifeiyinyue.top

[J02] 格式化输出
来源：http://dzk.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqo.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wbj.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wob.xuetiantiany.cn

TS:   d.toISOString()
来源：http://yxt.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://upm.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdl.yangfankeji.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://idf.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bkd.fehbvm.com

[J03] 字符串解析为日期
来源：http://mtv.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bua.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qpj.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://qbg.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://gqr.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://cvd.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lrh.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://mlf.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ucj.bbcook.cn

[J04] 时间戳与日期互转
来源：http://szf.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epk.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dng.ivvv.top


<!-- 参考信息 -->