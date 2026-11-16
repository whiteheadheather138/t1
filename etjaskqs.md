代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hee.xziqi.cn

[G07] 调用父类方法
来源：http://rlt.yuanzhike.top

Py:   super().greet()
来源：http://aza.zhengqikj.top

PHP:  parent::greet();
来源：http://zcz.sufxvd.cn

JS:   super.greet();
来源：http://hyi.gogol.net.cn

TS:   super.greet();
来源：http://nzi.birdmap.top

Java: super.greet();
来源：http://bdo.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gzu.zhiwuduotai.top

Ruby: super
来源：http://wjs.snrcjt.cn

C#:   base.Greet();
来源：http://fat.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://oik.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fdj.chenzaomai.com

PHP:  public static function f() {}
来源：http://rgj.yanxiufei.cn

JS:   static f() {}
来源：http://wve.yonumen.top

TS:   static f(): void {}
来源：http://jnr.hysaishi.cn

Java: static void f() {}
来源：http://blx.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://evp.ppjwa.cn

Ruby: def self.f; end
来源：http://fee.nanxuanxn.top

C#:   public static void F() {}
来源：http://qyw.yuxming.cn

[G09] 接口 / 抽象类
来源：http://trx.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://qna.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nuj.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://akf.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://xsq.tian-w.cn

Java: interface Shape { double area(); }
来源：http://ljl.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://peg.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nvh.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://ota.ehwqpu.com

[G10] 访问控制
来源：http://idg.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://itr.jiagoushi.top

PHP:  public / protected / private
来源：http://shs.meibo888.top

JS:   #private 字段；其余公开
来源：http://mfc.zdbjq.cn

TS:   public / protected / private
来源：http://gtc.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://kza.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rxv.9152youxi.cn

Ruby: public / protected / private
来源：http://zoq.gzhubu.top

C#:   public / protected / private / internal
来源：http://jqc.aibaodan.cn

[G11] getter / setter
来源：http://eld.pycfn.com

Py:   @property 与 @x.setter
来源：http://kav.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://llk.epnwcf.com

JS:   get name() { return this._name; }
来源：http://mbf.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://mpe.smart0.xyz

Java: public String getName() { return name; }
来源：http://ijc.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://sbc.yueranfly.top

Ruby: attr_accessor :name
来源：http://rma.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://kqu.tianlin.xyz

[G12] 对象转字符串
来源：http://jnx.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://bzn.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uel.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://dpu.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://bsf.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://mps.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://igr.hcnkem.com

Ruby: def to_s; @name; end
来源：http://dfz.tarul.cn

C#:   public override string ToString() => Name;
来源：http://zpn.guowangkeji.top

[G13] 判断对象类型
来源：http://eiy.birdmap.top

Py:   isinstance(u, User)
来源：http://oex.fktsv.cn

PHP:  $u instanceof User
来源：http://zee.kuanghao11.cn

JS:   u instanceof User
来源：http://itw.316326.xyz

TS:   u instanceof User
来源：http://tnl.zdqjudy.top

Java: u instanceof User
来源：http://ide.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pfw.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://qgn.guowangkeji.top

C#:   u is User
来源：http://dzq.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://rkh.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vhp.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://uof.jiagoushi.top

JS:   // 无内置：普通类或对象字面量
来源：http://omp.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://mrj.yuxming.cn

Java: record User(String name, int age) {}
来源：http://rhe.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://okn.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pvi.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://gol.chenjidiqi.icu

[G15] 枚举
来源：http://cqo.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://okk.hfpthk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wgz.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uri.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cep.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://ixl.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wcl.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://gbv.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dzx.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://ine.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rlq.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://cza.hammf.cn

JS:   Object.entries(obj)
来源：http://gqe.birdmap.top

TS:   Object.entries(obj)
来源：http://www.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gha.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oet.snrcjt.cn

Ruby: obj.instance_variables
来源：http://tec.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://cfu.sweek.top

================================================================================
来源：http://ovn.ydjk.org.cn

H. 异常与错误处理
来源：http://itt.yj20258.top

================================================================================
来源：http://car.yj20258.top

[H01] try / catch 基础
来源：http://ohj.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ehr.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqt.fengsongda.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mez.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xte.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://skj.yuanzhike.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mlk.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gcc.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://poo.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://iim.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bzl.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eef.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://ysa.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eqb.nanxuanxn.top

Java: try { f(); } finally { cleanup(); }
来源：http://uks.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jfz.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lut.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hvl.bjfxy.top

[H03] 主动抛出异常
来源：http://muw.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://tip.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uho.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://soi.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://qpz.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rwm.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssr.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://exk.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://lrp.yonumen.top

[H04] 自定义异常类型
来源：http://gbl.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://vqj.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://eig.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://xhl.fktsv.cn

TS:   class MyError extends Error {}
来源：http://nrp.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://fyr.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oei.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://upx.tanke756.top

C#:   class MyException : Exception {}
来源：http://vnv.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://srl.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://nch.kuanghao11.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kxv.xinyue.icu

JS:   if (e instanceof TypeError) {}
来源：http://eiq.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://suo.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://mfj.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://msa.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://ypb.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dhb.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://dsc.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://byf.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://htr.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nzn.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eir.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pjo.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oav.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://gea.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://rxx.chenjidiqi.icu

[H07] 断言
来源：http://cyq.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://hxn.gzhubu.top

PHP:  assert($x > 0);
来源：http://pde.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://cma.316326.xyz

TS:   console.assert(x > 0);
来源：http://nmu.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://ydu.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ecp.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ams.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://npi.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://upe.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://log.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jhi.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://hvo.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqo.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rhp.cdnleiting.top

Go:   err.Error()
来源：http://ysc.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://hfh.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://pfi.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://nlb.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gqo.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://khl.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://asl.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ktm.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vwi.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jdd.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://npr.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cbk.wangdashe.top

[H10] 资源自动释放
来源：http://mun.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jnp.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nox.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://llb.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dkx.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jam.aibaodan.cn

Go:   defer f.Close()
来源：http://gdu.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bgw.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yld.meibo888.top

================================================================================
来源：http://njo.tanke756.top

I. 正则表达式
来源：http://ske.gzhubu.top

================================================================================
来源：http://oic.jlsjyb.cn

[I01] 判断是否匹配
来源：http://dkl.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rkn.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://opn.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://tjj.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://awt.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yfl.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kip.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://lpy.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rjg.zycfv.cn

[I02] 提取所有匹配
来源：http://dhw.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://vso.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wml.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://odc.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://lkp.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyt.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mir.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://nyd.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nsm.hammf.cn

[I03] 提取捕获分组
来源：http://dir.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://afg.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cmz.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rph.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://toz.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://spl.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kxf.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lvs.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://efj.haohaochexian.top

[I04] 正则替换
来源：http://ikz.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jjd.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ece.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://nua.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://psv.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndi.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cmh.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jbc.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ave.snrcjt.cn

[I05] 按正则拆分
来源：http://yyt.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://dbt.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dwi.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://jej.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://byd.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://hil.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tbm.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://irt.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iyq.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rdl.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mae.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kig.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://edq.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vlk.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mkj.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ezk.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://byn.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://llh.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://ppa.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tiu.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mbx.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xxa.yanxiufei.cn

TS:   /error/gim
来源：http://uvt.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kev.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijt.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://zqn.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://laz.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://hkm.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mof.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pri.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://prq.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aaa.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://kii.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://awg.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uxo.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://res.ywan-chungtsiang.top

================================================================================
来源：http://jhu.guannengcc.top

J. 日期与时间
来源：http://var.chenzaomai.com

================================================================================
来源：http://zgb.aizwys.cn

[J01] 获取当前时间
来源：http://aas.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gxh.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yaw.ydzc1.top

JS:   new Date();  Date.now()
来源：http://tqq.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://ypd.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qan.sjlbkw.cn

Go:   time.Now()
来源：http://got.bbcook.cn

Ruby: Time.now
来源：http://ctr.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lir.dianchejie.cn

[J02] 格式化输出
来源：http://rvs.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gcd.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://esb.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://myy.gotoacloud.top

TS:   d.toISOString()
来源：http://zhf.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mkm.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vci.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zmp.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jek.yuxming.cn

[J03] 字符串解析为日期
来源：http://nzu.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vvn.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://umj.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://rui.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://uhg.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ksu.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tmj.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://nal.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rrs.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://pic.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://upx.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lsz.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clg.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fnu.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exu.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uah.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqs.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wrh.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://eur.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://wir.zhoulong.xyz


<!-- 参考信息 -->