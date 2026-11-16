代发 wailian999

JS:   this.name = "x";
来源：http://ltk.epnwcf.com

TS:   name: string = "x";
来源：http://quv.guowangkeji.top

Java: private String name;
来源：http://rcl.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdb.xylfe.cn

Ruby: @name = "x"
来源：http://qvt.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://aoo.fehbvm.com

[G04] 定义方法
来源：http://tyu.xinyue.icu

Py:   def greet(self): return self.name
来源：http://dvs.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ena.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://rcq.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://lnr.hesvh.cn

Java: String greet() { return name; }
来源：http://uol.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://whq.zhengqikj.top

Ruby: def greet; @name; end
来源：http://bjj.pycfn.com

C#:   public string Greet() => Name;
来源：http://qmw.jlsjyb.cn

[G05] 继承
来源：http://wij.nanxinkj.top

Py:   class Admin(User): pass
来源：http://rmw.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://jwf.fzhhl.top

JS:   class Admin extends User {}
来源：http://gng.shzxlz.cn

TS:   class Admin extends User {}
来源：http://rtp.sysykeji.top

Java: class Admin extends User {}
来源：http://yru.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://abo.hesvh.cn

Ruby: class Admin < User; end
来源：http://ihw.cheryme.top

C#:   class Admin : User {}
来源：http://wzj.fktsv.cn

[G06] 重写方法
来源：http://cxt.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://vdw.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vwf.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://unr.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://udu.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xhy.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fjv.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://jpk.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://yqd.birdmap.top

[G07] 调用父类方法
来源：http://jdw.pycfn.com

Py:   super().greet()
来源：http://vkn.ydjk.org.cn

PHP:  parent::greet();
来源：http://iyg.cqqwz.cn

JS:   super.greet();
来源：http://ggl.316326.xyz

TS:   super.greet();
来源：http://sxj.yuanzhike.top

Java: super.greet();
来源：http://dqw.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://acs.pengpengdd.cyou

Ruby: super
来源：http://myo.gzhubu.top

C#:   base.Greet();
来源：http://lgc.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://cvw.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mwh.ivvv.top

PHP:  public static function f() {}
来源：http://zxu.ydjk.org.cn

JS:   static f() {}
来源：http://apu.tian-w.cn

TS:   static f(): void {}
来源：http://kwz.jinyuanbaomall.cn

Java: static void f() {}
来源：http://jru.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gnm.ppjwa.cn

Ruby: def self.f; end
来源：http://qpa.chenzaomai.com

C#:   public static void F() {}
来源：http://iln.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://nom.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://zmt.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://val.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzi.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://myg.uphjek.com

Java: interface Shape { double area(); }
来源：http://mdq.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://and.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ifs.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://agb.yonumen.top

[G10] 访问控制
来源：http://htq.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://klz.tian-w.cn

PHP:  public / protected / private
来源：http://kpx.nwbrower.top

JS:   #private 字段；其余公开
来源：http://nsc.cdnleiting.top

TS:   public / protected / private
来源：http://byl.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://qzg.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://trh.gaohongyu789.top

Ruby: public / protected / private
来源：http://kxg.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://bdj.zdqjudy.top

[G11] getter / setter
来源：http://ywk.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://lqw.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gqr.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://ygl.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://tqf.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://wug.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xah.hywenlv.cn

Ruby: attr_accessor :name
来源：http://lbv.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://ebt.daria6918.cn

[G12] 对象转字符串
来源：http://hkn.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://beg.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://zjw.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://hdk.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://ejh.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://gze.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://wen.vehdjk.com

Ruby: def to_s; @name; end
来源：http://vxs.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://lwn.dianchejie.cn

[G13] 判断对象类型
来源：http://htf.nwbrower.top

Py:   isinstance(u, User)
来源：http://djf.nanxinkj.top

PHP:  $u instanceof User
来源：http://fiu.nanxinkj.top

JS:   u instanceof User
来源：http://jhh.yj202588.top

TS:   u instanceof User
来源：http://hgz.zhiwuduotai.top

Java: u instanceof User
来源：http://lyv.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aqu.mhx1999.top

Ruby: u.is_a?(User)
来源：http://jnh.chenzaomai.com

C#:   u is User
来源：http://inm.yj202588.top

[G14] 数据类 / record
来源：http://lcs.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kex.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://bcb.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://mhx.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://olg.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://ves.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://esb.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uif.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://anz.cucudq.cn

[G15] 枚举
来源：http://rpq.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utm.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fak.yj202588.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iyq.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bqt.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://fdh.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yaf.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://czc.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ebq.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://chb.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tde.sweek.top

PHP:  get_object_vars($obj);
来源：http://kqt.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://cju.hesvh.cn

TS:   Object.entries(obj)
来源：http://tyt.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ecb.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://rwu.shzxlz.cn

Ruby: obj.instance_variables
来源：http://qsg.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://qeh.daria6918.cn

================================================================================
来源：http://hrb.gotoacloud.top

H. 异常与错误处理
来源：http://mis.bjfxy.top

================================================================================
来源：http://ddw.ybcxt.top

[H01] try / catch 基础
来源：http://qks.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yrf.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cdu.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nze.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://goz.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kjf.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://quv.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cce.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uyb.daxiang520.top

[H02] finally / ensure 收尾
来源：http://nqy.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://nxq.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ezd.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fom.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mxh.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bdp.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rth.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fgh.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ksv.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://snx.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://eld.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fto.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://efu.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://hty.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fxg.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dwm.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ckr.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://vvi.jqgufenzy.top

[H04] 自定义异常类型
来源：http://eug.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://crg.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://los.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://wnn.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://yvp.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://mvc.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kdp.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://luc.xziqi.cn

C#:   class MyException : Exception {}
来源：http://fus.ppjwa.cn

[H05] 捕获特定类型
来源：http://osc.tianlin.xyz

Py:   except ValueError as e:
来源：http://cve.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lit.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://jmr.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://auo.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://pjn.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://daj.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://duj.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://efu.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://qvl.cheryme.top

Py:   value = d.get("k") or default
来源：http://vko.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://esr.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://nso.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://zdp.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lme.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fyp.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ozs.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://wwr.xylfe.cn

[H07] 断言
来源：http://ons.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://fmo.ehwqpu.com

PHP:  assert($x > 0);
来源：http://rch.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://zlm.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://swd.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://xgs.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yvc.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://uwy.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://rki.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://hov.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://pyx.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gde.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://gyi.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wbk.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cob.yj20258888.top

Go:   err.Error()
来源：http://lwj.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://nsc.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://hgb.yuanzhike.top

[H09] 带错误码的异常
来源：http://vhp.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://puj.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cye.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hbh.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmx.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tem.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nng.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://evl.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kea.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://wvl.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wtr.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://idp.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyf.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rri.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kkt.yj202588.top

Go:   defer f.Close()
来源：http://nym.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fnj.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rdi.yfazqb.com

================================================================================
来源：http://xli.xuanzx.com

I. 正则表达式
来源：http://uya.hnqzz.top

================================================================================
来源：http://mnl.jqgfzy.top

[I01] 判断是否匹配
来源：http://sys.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ggm.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://chg.vehdjk.com

JS:   /\d+/.test(s)
来源：http://wgi.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://qqx.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hgu.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ayb.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://ujs.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://adl.jiagoushi.top

[I02] 提取所有匹配
来源：http://iow.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://fyu.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://otr.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://azw.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://tuv.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zne.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oac.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://xcd.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lgi.jqgfzy.top

[I03] 提取捕获分组
来源：http://ryw.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dsh.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://akh.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://abx.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xer.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qwo.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ofo.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kju.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uhd.havefunace.top

[I04] 正则替换
来源：http://bqg.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jlv.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yww.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://spl.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://bvl.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xxx.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sym.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qrv.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xbq.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://lod.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jqa.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hay.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://grp.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://yrn.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ewz.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gtm.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://qzr.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rcx.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pza.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vbv.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fse.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uba.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://adt.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://apd.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwq.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wjl.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ajg.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://vjd.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bol.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxf.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zre.shanyushiyangkeji.top

TS:   /error/gim
来源：http://hoa.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yus.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iwq.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://hth.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rql.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://yjx.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bir.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uah.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pts.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kqf.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qly.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sve.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lcf.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pcs.dashuyun.cn

================================================================================
来源：http://jxu.tian-w.cn

J. 日期与时间
来源：http://jjl.jyoumei.cn

================================================================================
来源：http://vbv.yfazqb.com

[J01] 获取当前时间
来源：http://xvu.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lfh.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://axm.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://swo.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://gvi.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://deu.hnqzz.top


<!-- 参考信息 -->