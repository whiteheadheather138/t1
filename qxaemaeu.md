代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://cac.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://umk.bbcook.cn

C#:   public string Greet() => Name;
来源：http://toy.zycfv.cn

[G05] 继承
来源：http://eeq.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://cds.yuxming.cn

PHP:  class Admin extends User {}
来源：http://olm.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://igt.daria6918.cn

TS:   class Admin extends User {}
来源：http://jdw.meibo888.top

Java: class Admin extends User {}
来源：http://mrh.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rkn.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://yhi.fengsongda.top

C#:   class Admin : User {}
来源：http://fdw.jlsjyb.cn

[G06] 重写方法
来源：http://obe.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://hxv.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zdm.uphjek.com

JS:   greet() { return "admin"; }
来源：http://vrg.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://tqu.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://yqu.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://psn.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://eoh.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://aaq.yueranfly.top

[G07] 调用父类方法
来源：http://riw.vehdjk.com

Py:   super().greet()
来源：http://mab.zhengqikj.top

PHP:  parent::greet();
来源：http://yqc.gzhubu.top

JS:   super.greet();
来源：http://ihu.jinqigufen.top

TS:   super.greet();
来源：http://yom.nanxuanxn.top

Java: super.greet();
来源：http://vus.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gbl.havefunace.top

Ruby: super
来源：http://udd.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://ijf.bjfxy.top

[G08] 静态方法与属性
来源：http://rcp.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hfo.fehbvm.com

PHP:  public static function f() {}
来源：http://gss.yj202588.top

JS:   static f() {}
来源：http://rjz.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://yzi.tian-w.cn

Java: static void f() {}
来源：http://guv.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lpw.pengpengdd.cyou

Ruby: def self.f; end
来源：http://qvi.gotoacloud.top

C#:   public static void F() {}
来源：http://erx.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://gvi.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://wfp.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://thk.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rrx.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://iva.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://ijh.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://qwn.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jwo.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://oqq.shanyushiyangkeji.top

[G10] 访问控制
来源：http://nqi.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://vrl.jqgufenzy.top

PHP:  public / protected / private
来源：http://kvv.yfazqb.com

JS:   #private 字段；其余公开
来源：http://slo.cucudq.cn

TS:   public / protected / private
来源：http://evq.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://imp.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://awf.0kj1m.cn

Ruby: public / protected / private
来源：http://xqn.9152youxi.cn

C#:   public / protected / private / internal
来源：http://dgu.yanxiufei.cn

[G11] getter / setter
来源：http://tbq.hnqzz.top

Py:   @property 与 @x.setter
来源：http://vhf.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://act.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://flg.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://yax.mhx1999.top

Java: public String getName() { return name; }
来源：http://tkk.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://efl.hysaishi.cn

Ruby: attr_accessor :name
来源：http://vmc.mhx1999.top

C#:   public string Name { get; set; }
来源：http://dbd.nwbrower.top

[G12] 对象转字符串
来源：http://jfk.tanke756.top

Py:   def __str__(self): return self.name
来源：http://mkj.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://hnm.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://zlq.pengpengdd.cyou

TS:   toString(): string { return this.name; }
来源：http://ddo.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://gml.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://arn.yj20258.top

Ruby: def to_s; @name; end
来源：http://yzl.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://ryw.feifeiyinyue.top

[G13] 判断对象类型
来源：http://myw.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://ckx.svipenyu.cn

PHP:  $u instanceof User
来源：http://fim.zdqjudy.top

JS:   u instanceof User
来源：http://idx.ctjpmb.com

TS:   u instanceof User
来源：http://jvp.hysaishi.cn

Java: u instanceof User
来源：http://pvf.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rgi.hcnkem.com

Ruby: u.is_a?(User)
来源：http://uwg.zhoulong.xyz

C#:   u is User
来源：http://gpy.nwbrower.top

[G14] 数据类 / record
来源：http://mxi.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://awu.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://imb.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://rzk.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://pqp.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://ite.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://bgd.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://axj.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://fgn.yanxiufei.cn

[G15] 枚举
来源：http://kzc.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wbn.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qml.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gau.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hss.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://ysc.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ged.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://jzr.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ghy.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://oqt.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cfw.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://jdb.xziqi.cn

JS:   Object.entries(obj)
来源：http://cax.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://zss.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tiw.zdqjudy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yjf.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://yne.pycfn.com

C#:   // 用反射或 System.Text.Json
来源：http://bye.316326.xyz

================================================================================
来源：http://yfe.yvedp.cn

H. 异常与错误处理
来源：http://ata.cdnleiting.top

================================================================================
来源：http://lhd.tianlin.xyz

[H01] try / catch 基础
来源：http://cze.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ziy.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwh.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ytm.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tam.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://idr.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fxx.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rcx.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qzq.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://ead.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://wrn.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://qbf.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uhe.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hit.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ysl.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yzx.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nky.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jqc.jinqigufen.top

[H03] 主动抛出异常
来源：http://zla.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://vzv.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ide.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://obj.cheryme.top

TS:   throw new Error("错误信息");
来源：http://jwd.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gnd.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssn.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uyp.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://lif.hysaishi.cn

[H04] 自定义异常类型
来源：http://cyw.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://oil.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://iyj.mhx1999.top

JS:   class MyError extends Error {}
来源：http://awi.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://hou.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://abr.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fwq.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://rme.birdmap.top

C#:   class MyException : Exception {}
来源：http://zio.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://gdg.yonumen.top

Py:   except ValueError as e:
来源：http://tpp.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://poo.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://nmw.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://cwm.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://iol.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://muy.sweek.top

Ruby: rescue ArgumentError => e
来源：http://lfu.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zog.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://olg.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://qzi.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tch.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://tgl.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://rln.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sqe.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fdx.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://rht.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://sej.vehdjk.com

[H07] 断言
来源：http://lqo.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://vbl.epnwcf.com

PHP:  assert($x > 0);
来源：http://jzg.fzhhl.top

JS:   console.assert(x > 0);
来源：http://pxx.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://gmw.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://wad.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rzw.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://agl.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://qvi.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://ama.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://yqe.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gbo.xuanzx.com

JS:   e.message;  e.stack
来源：http://dgh.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rqy.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uds.yonumen.top

Go:   err.Error()
来源：http://xcn.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://htt.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://aqh.ctjpmb.com

[H09] 带错误码的异常
来源：http://pot.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://anj.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yiq.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lxh.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://exc.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://apf.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aih.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://czw.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://irn.sxryk.cn

[H10] 资源自动释放
来源：http://mzq.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zff.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nss.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fbl.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qeg.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fuu.aizwys.cn

Go:   defer f.Close()
来源：http://ice.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vrv.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bkw.wangshuangyany.cn

================================================================================
来源：http://dnd.shzxlz.cn

I. 正则表达式
来源：http://onb.xziqi.cn

================================================================================
来源：http://sol.hesvh.cn

[I01] 判断是否匹配
来源：http://zqv.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://seb.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kik.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://icv.c1oappe.top

TS:   /\d+/.test(s)
来源：http://jco.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vgt.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://csq.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://ott.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wmv.guannengcc.top

[I02] 提取所有匹配
来源：http://zbe.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://rwl.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jbi.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lvz.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://rli.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ldr.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wmx.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://kzv.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ukm.ydjk.org.cn

[I03] 提取捕获分组
来源：http://sjw.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bul.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kps.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hpy.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://exr.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qqi.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://txn.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dyq.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bws.gaohongyu789.top

[I04] 正则替换
来源：http://mzr.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pfx.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dhp.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cfg.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://amr.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kmo.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mng.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nmp.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vzk.c1oappe.top

[I05] 按正则拆分
来源：http://zxv.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gzf.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://swn.sxryk.cn

JS:   s.split(/\s*,\s*/)
来源：http://jjp.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://bkb.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://hwf.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://laz.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://omy.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wmc.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yii.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fkp.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aum.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xcb.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rys.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qeg.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aqa.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kmf.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tmp.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://wwb.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://afp.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wch.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdu.yanxiufei.cn

TS:   /error/gim
来源：http://kfg.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vgm.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ozk.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://gjw.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://afq.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://mle.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rct.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vgv.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sod.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mnh.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dqa.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nuo.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://esi.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pod.iojbl.cn

================================================================================
来源：http://zam.xuetiantiany.cn

J. 日期与时间
来源：http://iva.tarul.cn

================================================================================
来源：http://qlf.ctjpmb.com

[J01] 获取当前时间
来源：http://hyg.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vuv.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dky.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://exn.meibo888.top

TS:   new Date();  Date.now()
来源：http://bcj.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pkm.zhongyouzk.top

Go:   time.Now()
来源：http://jci.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://gca.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tqn.yuxming.cn

[J02] 格式化输出
来源：http://smd.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhh.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://abx.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uuf.gaohongyu789.top

TS:   d.toISOString()
来源：http://syf.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wey.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wuk.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hot.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vny.yangfankeji.com


<!-- 参考信息 -->