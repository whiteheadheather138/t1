代发 wailian999

Py:   class Admin(User): pass
来源：http://orc.cheryme.top

PHP:  class Admin extends User {}
来源：http://gmc.shuidangran.top

JS:   class Admin extends User {}
来源：http://igs.yangfankeji.com

TS:   class Admin extends User {}
来源：http://btg.jinqigfzy.top

Java: class Admin extends User {}
来源：http://ojy.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mlu.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://pxe.aibaodan.cn

C#:   class Admin : User {}
来源：http://rba.ydzc1.top

[G06] 重写方法
来源：http://jvi.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://vmd.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://skg.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://mnf.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://hjx.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://rbi.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://her.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://upe.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://rqr.vehdjk.com

[G07] 调用父类方法
来源：http://xbm.zdbjq.cn

Py:   super().greet()
来源：http://egh.daria6918.cn

PHP:  parent::greet();
来源：http://ydm.epnwcf.com

JS:   super.greet();
来源：http://wvf.yfazqb.com

TS:   super.greet();
来源：http://eng.ydzc1.top

Java: super.greet();
来源：http://uaj.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lud.jqgfzy.top

Ruby: super
来源：http://tdx.hongshengwenyu.top

C#:   base.Greet();
来源：http://clz.cqqwz.cn

[G08] 静态方法与属性
来源：http://rcg.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ubp.fehbvm.com

PHP:  public static function f() {}
来源：http://mjd.jiagoushi.top

JS:   static f() {}
来源：http://msf.pycfn.com

TS:   static f(): void {}
来源：http://qxz.daria6918.cn

Java: static void f() {}
来源：http://rsy.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hxu.smart0.xyz

Ruby: def self.f; end
来源：http://hmt.hywenlv.cn

C#:   public static void F() {}
来源：http://zgt.xylfe.cn

[G09] 接口 / 抽象类
来源：http://qrb.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://kgy.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bid.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kxf.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://ltm.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://jhu.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://xlp.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oam.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://khi.hammf.cn

[G10] 访问控制
来源：http://nwt.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://yqx.epnwcf.com

PHP:  public / protected / private
来源：http://vyl.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://nzm.smart0.xyz

TS:   public / protected / private
来源：http://ncq.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://dfy.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uzg.zhiwuduotai.top

Ruby: public / protected / private
来源：http://qlr.cdnleiting.top

C#:   public / protected / private / internal
来源：http://kdw.vqdsnc.cn

[G11] getter / setter
来源：http://guq.guannengcc.top

Py:   @property 与 @x.setter
来源：http://cte.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rxw.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://uas.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://fcd.52xcode.cn

Java: public String getName() { return name; }
来源：http://nhf.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gzm.sweek.top

Ruby: attr_accessor :name
来源：http://ezg.pycfn.com

C#:   public string Name { get; set; }
来源：http://zvx.sxryk.cn

[G12] 对象转字符串
来源：http://gea.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://ssf.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hzy.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://tms.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://oaq.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://vtg.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ikt.sysykeji.top

Ruby: def to_s; @name; end
来源：http://rlp.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://xaa.sysykeji.top

[G13] 判断对象类型
来源：http://cfl.gotoacloud.top

Py:   isinstance(u, User)
来源：http://klt.cucudq.cn

PHP:  $u instanceof User
来源：http://olq.daria6918.cn

JS:   u instanceof User
来源：http://qyc.zhengqikj.top

TS:   u instanceof User
来源：http://sxq.redwolf501.top

Java: u instanceof User
来源：http://grv.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://lwt.yonumen.top

Ruby: u.is_a?(User)
来源：http://cei.jinghuilouyu.cn

C#:   u is User
来源：http://fmx.sufxvd.cn

[G14] 数据类 / record
来源：http://jwy.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jca.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://tet.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ctw.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://fwx.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://zsg.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://akm.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rtq.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://obq.hcnkem.com

[G15] 枚举
来源：http://kvl.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rog.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tyv.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fsv.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wdv.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://qiq.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cka.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://cfc.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vuu.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://liw.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lhk.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://dex.nwbrower.top

JS:   Object.entries(obj)
来源：http://agq.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://dlv.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cll.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tls.tanke756.top

Ruby: obj.instance_variables
来源：http://nvn.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://uma.yuxming.cn

================================================================================
来源：http://yha.fehbvm.com

H. 异常与错误处理
来源：http://mvu.tianlin.xyz

================================================================================
来源：http://llj.316326.xyz

[H01] try / catch 基础
来源：http://ylg.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pcv.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xmx.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gee.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rsk.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rhu.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uea.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fnf.yuxming.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mbt.aizwys.cn

[H02] finally / ensure 收尾
来源：http://qmq.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jcl.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hma.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vlp.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ors.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://peg.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bwa.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vuf.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gsh.ppjwa.cn

[H03] 主动抛出异常
来源：http://yiy.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://ufu.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://efr.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://yox.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://hxn.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jfx.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nhb.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tkw.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://kde.havefunace.top

[H04] 自定义异常类型
来源：http://rst.uphjek.com

Py:   class MyError(Exception): pass
来源：http://yfb.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lse.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://jha.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://azl.ppjwa.cn

Java: class MyException extends RuntimeException {}
来源：http://ypb.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://duj.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://ypi.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://new.ydzc1.top

[H05] 捕获特定类型
来源：http://uxk.jianghu66.top

Py:   except ValueError as e:
来源：http://kdv.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bks.daxiang520.top

JS:   if (e instanceof TypeError) {}
来源：http://ncj.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://udj.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://aik.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wab.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://lwf.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rbz.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://tiy.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://lug.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://imm.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://lpf.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bye.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fyk.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://rzd.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://ncl.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://lkx.zhaomingkeji.xyz

[H07] 断言
来源：http://pzk.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://kqu.cashguo.top

PHP:  assert($x > 0);
来源：http://fyi.aizwys.cn

JS:   console.assert(x > 0);
来源：http://hnn.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://nbj.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://jfg.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xji.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://scn.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://gab.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://uoz.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://moc.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uww.52xcode.cn

JS:   e.message;  e.stack
来源：http://eng.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://hdf.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ymc.yangfankeji.com

Go:   err.Error()
来源：http://olz.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://dhm.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://ude.vehdjk.com

[H09] 带错误码的异常
来源：http://rvg.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yei.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pxp.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aap.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tie.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drb.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tep.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cno.xziqi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kfz.ydzc1.top

[H10] 资源自动释放
来源：http://xct.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://npx.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lsc.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vtm.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://koi.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cff.daxiang520.top

Go:   defer f.Close()
来源：http://tvh.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zvb.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rci.sxryk.cn

================================================================================
来源：http://tes.dianchejie.cn

I. 正则表达式
来源：http://hiw.yj20258.top

================================================================================
来源：http://yoy.sxryk.cn

[I01] 判断是否匹配
来源：http://ege.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yqo.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wfe.316326.xyz

JS:   /\d+/.test(s)
来源：http://gmu.ydzc1.top

TS:   /\d+/.test(s)
来源：http://rcl.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lrh.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ghg.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://dub.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tzw.hywenlv.cn

[I02] 提取所有匹配
来源：http://wbm.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://tsh.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tfm.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rcs.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://ehe.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ukx.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fdu.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://nma.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tox.xylfe.cn

[I03] 提取捕获分组
来源：http://ymd.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wlo.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pqp.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://idr.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qek.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://got.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qac.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwo.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zmv.sweek.top

[I04] 正则替换
来源：http://guf.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fmr.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://epz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://upq.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uop.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dmb.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ujb.smart0.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://fir.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aum.ctjpmb.com

[I05] 按正则拆分
来源：http://sbx.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fba.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qql.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://dwz.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://dyi.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://stn.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ykd.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://aim.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nug.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ash.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gyl.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tqn.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmz.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oad.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zoy.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iqi.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://glp.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qji.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://wql.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bzn.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://anw.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ynr.bbcook.cn

TS:   /error/gim
来源：http://txq.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yik.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bim.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://ktj.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qvs.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://nnq.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://thm.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bdb.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qga.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bis.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sna.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ehe.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ulg.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://spl.xuanzx.com

================================================================================
来源：http://pgp.hnxiangtu.top

J. 日期与时间
来源：http://uuy.quarkkingdee.top

================================================================================
来源：http://ocj.tanke756.top

[J01] 获取当前时间
来源：http://ycv.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://toi.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://twm.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://qfk.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://tnc.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lhm.epnwcf.com

Go:   time.Now()
来源：http://rmw.vqdsnc.cn

Ruby: Time.now
来源：http://dpc.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://txi.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://pqk.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xgs.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ajx.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://psr.jiagoushi.top

TS:   d.toISOString()
来源：http://hvr.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ovy.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zqb.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpi.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cru.gzhubu.top

[J03] 字符串解析为日期
来源：http://rvr.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hoh.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qej.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://xym.0kj1m.cn


<!-- 参考信息 -->