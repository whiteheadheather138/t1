代发 wailian999

Java: class Admin extends User {}
来源：http://gdw.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mbw.nwbrower.top

Ruby: class Admin < User; end
来源：http://fzi.sysykeji.top

C#:   class Admin : User {}
来源：http://nmb.bbcook.cn

[G06] 重写方法
来源：http://gim.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://ytj.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aua.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://ihn.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://dir.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://yia.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mya.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://geh.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://ecq.xinyue.icu

[G07] 调用父类方法
来源：http://zkn.0kj1m.cn

Py:   super().greet()
来源：http://epz.daria6918.cn

PHP:  parent::greet();
来源：http://roe.jianghu66.top

JS:   super.greet();
来源：http://sem.andypj.xyz

TS:   super.greet();
来源：http://sqx.wangdashe.top

Java: super.greet();
来源：http://arf.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iqs.cdnleiting.top

Ruby: super
来源：http://keq.cashguo.top

C#:   base.Greet();
来源：http://wru.ppjwa.cn

[G08] 静态方法与属性
来源：http://dhi.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aee.yvedp.cn

PHP:  public static function f() {}
来源：http://syl.sxryk.cn

JS:   static f() {}
来源：http://bmx.hongshengwenyu.top

TS:   static f(): void {}
来源：http://nwo.uphjek.com

Java: static void f() {}
来源：http://nwc.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rfm.ydzc1.top

Ruby: def self.f; end
来源：http://fxe.hnxiangtu.top

C#:   public static void F() {}
来源：http://pvw.yvedp.cn

[G09] 接口 / 抽象类
来源：http://vaw.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://fcv.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://sex.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kya.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://rfq.jinqigfzy.top

Java: interface Shape { double area(); }
来源：http://qie.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://yre.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://slw.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://rke.sysykeji.top

[G10] 访问控制
来源：http://kou.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://klm.jianghu66.top

PHP:  public / protected / private
来源：http://cis.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://rxc.yvedp.cn

TS:   public / protected / private
来源：http://elx.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://tyg.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://fyn.haohaochexian.top

Ruby: public / protected / private
来源：http://yub.bbcook.cn

C#:   public / protected / private / internal
来源：http://cjt.vehdjk.com

[G11] getter / setter
来源：http://imm.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://jvh.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zjm.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://zqn.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://vcm.gzhubu.top

Java: public String getName() { return name; }
来源：http://ero.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qts.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://irz.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://ygj.smart0.xyz

[G12] 对象转字符串
来源：http://cqq.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://yrt.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bgs.316326.xyz

JS:   toString() { return this.name; }
来源：http://dzl.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://ldr.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://mja.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://gsf.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://lwg.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://kpi.hywenlv.cn

[G13] 判断对象类型
来源：http://miv.tanke756.top

Py:   isinstance(u, User)
来源：http://agu.316326.xyz

PHP:  $u instanceof User
来源：http://cwb.epnwcf.com

JS:   u instanceof User
来源：http://ply.uphjek.com

TS:   u instanceof User
来源：http://pdp.shuidangran.top

Java: u instanceof User
来源：http://syk.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dbs.gzhubu.top

Ruby: u.is_a?(User)
来源：http://jjj.gogol.net.cn

C#:   u is User
来源：http://ibz.cqqwz.cn

[G14] 数据类 / record
来源：http://thg.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qey.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://rfw.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xfc.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://mgq.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://yrp.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://euu.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://njq.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://pao.shuidangran.top

[G15] 枚举
来源：http://jfe.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khy.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pcs.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lto.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cdm.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://jdd.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xuz.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://yus.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ibu.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://ulh.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eii.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://fse.yuxming.cn

JS:   Object.entries(obj)
来源：http://ffs.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://atg.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uwq.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://epo.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://tmt.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://wua.fengsongda.top

================================================================================
来源：http://dgx.bbcook.cn

H. 异常与错误处理
来源：http://aln.cashguo.top

================================================================================
来源：http://ydm.sweek.top

[H01] try / catch 基础
来源：http://bhk.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vru.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://swt.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lst.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jad.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wbt.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kss.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eot.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bbu.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://dmx.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://chl.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://rny.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jtg.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vlj.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://zzo.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://jxt.ydjk.org.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://udx.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tjj.andypj.xyz

[H03] 主动抛出异常
来源：http://dkt.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://cwk.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dtc.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://tsq.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://bys.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gps.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpk.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yoc.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://kyi.jiagoushi.top

[H04] 自定义异常类型
来源：http://uii.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://yyp.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mqf.c1oappe.top

JS:   class MyError extends Error {}
来源：http://clj.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://onk.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://qpv.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yvt.shuidangran.top

Ruby: class MyError < StandardError; end
来源：http://ini.andypj.xyz

C#:   class MyException : Exception {}
来源：http://rct.hywenlv.cn

[H05] 捕获特定类型
来源：http://vlp.yueranfly.top

Py:   except ValueError as e:
来源：http://xcu.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ijm.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://qsl.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://muh.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://uzj.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://guz.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://hnd.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://geh.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://fsq.tian-w.cn

Py:   value = d.get("k") or default
来源：http://bmx.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://psm.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://pxp.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://ivl.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gwb.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://est.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://zum.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://dhz.xuanzx.com

[H07] 断言
来源：http://fcv.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://tou.hammf.cn

PHP:  assert($x > 0);
来源：http://azx.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://krg.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://kai.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://kta.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uef.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://krn.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://hmy.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://icm.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://scj.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gnl.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://qct.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tdn.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://quh.fktsv.cn

Go:   err.Error()
来源：http://ukg.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://dbr.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://aqb.ppjwa.cn

[H09] 带错误码的异常
来源：http://mfk.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sfp.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ftc.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezo.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nsb.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ugb.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://akr.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://txf.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://grf.sweek.top

[H10] 资源自动释放
来源：http://xmy.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zho.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sle.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tga.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sqj.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lpz.ydzc1.top

Go:   defer f.Close()
来源：http://hgm.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dgc.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://thm.cashguo.top

================================================================================
来源：http://kba.zhongyouzk.top

I. 正则表达式
来源：http://lva.shzxlz.cn

================================================================================
来源：http://ckc.jinqigufen.top

[I01] 判断是否匹配
来源：http://iwx.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://knb.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://jpd.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://pae.cashguo.top

TS:   /\d+/.test(s)
来源：http://djd.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://all.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ipw.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://ezw.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fdb.ctjpmb.com

[I02] 提取所有匹配
来源：http://ikd.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://ibf.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://btw.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxz.hammf.cn

TS:   s.match(/\d+/g)
来源：http://qdv.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://air.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hmx.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://xuj.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tjc.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://toz.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ogk.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://byh.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wac.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ekf.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dek.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ztc.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ate.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uri.shuidangran.top

[I04] 正则替换
来源：http://pqj.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://frq.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xrn.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://mlp.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hsl.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ypt.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://knq.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iau.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ria.cqqwz.cn

[I05] 按正则拆分
来源：http://xsk.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://opi.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://arq.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://vff.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://ich.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://xck.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nwn.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qmp.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xtv.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yhi.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://chd.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://smd.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpn.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lfa.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://srm.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxu.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iwp.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkk.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://cqu.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ody.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fyv.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhc.uphjek.com

TS:   /error/gim
来源：http://fko.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rno.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hbe.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://qjf.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctv.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://bzm.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://waq.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tib.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gnt.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcq.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ity.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxc.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xkg.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xmk.tarul.cn

================================================================================
来源：http://gxe.gotoacloud.top

J. 日期与时间
来源：http://obr.yueranfly.top

================================================================================
来源：http://dyr.cdnleiting.top

[J01] 获取当前时间
来源：http://vdz.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ffb.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vep.mhx1999.top

JS:   new Date();  Date.now()
来源：http://ryu.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://mzz.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://loi.cashguo.top

Go:   time.Now()
来源：http://mng.chenjidiqi.icu

Ruby: Time.now
来源：http://tua.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jvs.yonumen.top

[J02] 格式化输出
来源：http://xpq.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://goc.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ohc.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zbe.ivvv.top

TS:   d.toISOString()
来源：http://kkv.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xez.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ecq.jyoumei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blw.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://naw.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://rws.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yoi.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://htz.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://qks.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://hdh.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://uzh.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dec.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://ubu.sxryk.cn


<!-- 参考信息 -->