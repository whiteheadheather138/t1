代发 wailian999

JS:   super.greet();
来源：http://nux.shanyushiyangkeji.top

TS:   super.greet();
来源：http://bfn.shzxlz.cn

Java: super.greet();
来源：http://xad.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sua.haohaochexian.top

Ruby: super
来源：http://ctt.yuxming.cn

C#:   base.Greet();
来源：http://omn.wangdashe.top

[G08] 静态方法与属性
来源：http://zuz.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kfa.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://bfm.hesvh.cn

JS:   static f() {}
来源：http://rwu.sxryk.cn

TS:   static f(): void {}
来源：http://msa.hysaishi.cn

Java: static void f() {}
来源：http://blg.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kcc.ehwqpu.com

Ruby: def self.f; end
来源：http://rqt.hnqzz.top

C#:   public static void F() {}
来源：http://cne.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://lkt.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://uzq.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://aur.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nwn.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://fno.jianghu66.top

Java: interface Shape { double area(); }
来源：http://aqe.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://vys.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fuq.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://gob.c1oappe.top

[G10] 访问控制
来源：http://nzy.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://auv.fehbvm.com

PHP:  public / protected / private
来源：http://akq.nwbrower.top

JS:   #private 字段；其余公开
来源：http://tao.c1oappe.top

TS:   public / protected / private
来源：http://kmg.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://kwt.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kfw.ybcxt.top

Ruby: public / protected / private
来源：http://dey.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://bzz.yvedp.cn

[G11] getter / setter
来源：http://ait.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://tzk.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://apz.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://fym.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://tyo.shanyushiyangkeji.top

Java: public String getName() { return name; }
来源：http://lrk.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ptv.hongshengwenyu.top

Ruby: attr_accessor :name
来源：http://rzf.shuidangran.top

C#:   public string Name { get; set; }
来源：http://sww.andypj.xyz

[G12] 对象转字符串
来源：http://bbp.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://uht.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cry.ydzc1.top

JS:   toString() { return this.name; }
来源：http://zgu.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://fkp.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://xkw.ydjk.org.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mpo.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://toy.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://krx.redwolf501.top

[G13] 判断对象类型
来源：http://pwo.yueranfly.top

Py:   isinstance(u, User)
来源：http://uwr.52xcode.cn

PHP:  $u instanceof User
来源：http://bqv.0kj1m.cn

JS:   u instanceof User
来源：http://rux.52xcode.cn

TS:   u instanceof User
来源：http://emd.mhx1999.top

Java: u instanceof User
来源：http://vmv.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ycu.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://xrh.iojbl.cn

C#:   u is User
来源：http://bln.dashuyun.cn

[G14] 数据类 / record
来源：http://xbf.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nsj.svipenyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://cld.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cja.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://fec.yj202588.top

Java: record User(String name, int age) {}
来源：http://ixp.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://vdy.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqu.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://woq.fktsv.cn

[G15] 枚举
来源：http://ibl.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://emi.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dqc.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jqm.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jqo.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://szo.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fhb.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://qwf.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yik.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://dwi.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jie.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://snh.tarul.cn

JS:   Object.entries(obj)
来源：http://ifc.haohaochexian.top

TS:   Object.entries(obj)
来源：http://ijv.c1oappe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://byk.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hbv.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://vhj.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://lof.c1oappe.top

================================================================================
来源：http://sni.nanxuanxn.top

H. 异常与错误处理
来源：http://kzj.daxiang520.top

================================================================================
来源：http://fdc.xuanzx.com

[H01] try / catch 基础
来源：http://iad.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://izn.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hzz.jiagoushi.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yuq.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://buo.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wpq.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rdk.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://llu.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uwu.zhixingplan.top

[H02] finally / ensure 收尾
来源：http://mjn.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ien.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ahj.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pah.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dju.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://svb.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bdu.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://erk.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://elv.zdqjudy.top

[H03] 主动抛出异常
来源：http://dhc.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://xfy.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gjy.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://saz.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://itw.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://msy.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tag.jlsjyb.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tmr.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://gqe.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://vuj.yj202588.top

Py:   class MyError(Exception): pass
来源：http://pwb.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aee.xuanzx.com

JS:   class MyError extends Error {}
来源：http://kxs.wangdashe.top

TS:   class MyError extends Error {}
来源：http://ggw.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://vmt.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xop.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://gow.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://zvd.tarul.cn

[H05] 捕获特定类型
来源：http://vgl.ehwqpu.com

Py:   except ValueError as e:
来源：http://kli.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xgz.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://yfy.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://bvp.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://thl.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jop.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://eaa.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sxa.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://pqn.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://emh.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://zlk.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://frr.jinqigufen.top

TS:   obj?.a?.b;  d ?? default
来源：http://yhf.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jxr.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://roj.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://bes.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://tyj.yanxiufei.cn

[H07] 断言
来源：http://zpg.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://rfd.ivvv.top

PHP:  assert($x > 0);
来源：http://ymo.yj20258.top

JS:   console.assert(x > 0);
来源：http://qll.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://ses.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://wqp.svipenyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tij.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://dcl.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://zvx.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://tnu.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://vra.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qrz.zhengqikj.top

JS:   e.message;  e.stack
来源：http://ght.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ehs.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sdn.hnxiangtu.top

Go:   err.Error()
来源：http://jet.sweek.top

Ruby: e.message;  e.backtrace
来源：http://yvf.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://hsk.yj20258.top

[H09] 带错误码的异常
来源：http://byt.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vee.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://myr.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bsz.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://szi.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://avj.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://urt.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wak.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://spq.gotoacloud.top

[H10] 资源自动释放
来源：http://jax.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nuq.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cjw.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zya.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kkq.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kud.meibo888.top

Go:   defer f.Close()
来源：http://xhh.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ima.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wud.chenzaomai.com

================================================================================
来源：http://heg.zhengqikj.top

I. 正则表达式
来源：http://ycu.xuetiantiany.cn

================================================================================
来源：http://wum.yanxiufei.cn

[I01] 判断是否匹配
来源：http://dmn.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pri.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://bic.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://lud.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://qiq.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://elx.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fmw.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://fuj.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://urm.ehwqpu.com

[I02] 提取所有匹配
来源：http://ngc.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://gyj.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyv.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bjz.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://ttz.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rrc.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mcf.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://jrv.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zhi.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://oay.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jnp.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cik.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cfs.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gpn.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://llv.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ijx.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zhp.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wqs.chenlongwang.top

[I04] 正则替换
来源：http://aik.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bom.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lqv.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://zyx.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://hvq.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fno.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uhb.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ugm.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qye.meibo888.top

[I05] 按正则拆分
来源：http://urs.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xmz.hcnkem.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsu.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://otf.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://gaq.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://rvd.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dra.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://zql.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xxo.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ube.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dme.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wzu.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmu.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bxq.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogx.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ceh.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xor.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://com.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://wvw.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://frm.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kes.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nom.uphjek.com

TS:   /error/gim
来源：http://qse.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rwb.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cvq.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://lpf.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tae.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://gkd.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nza.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://clw.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cll.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vnk.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ddi.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://irc.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pqg.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rsv.hysaishi.cn

================================================================================
来源：http://hpp.hongshengwenyu.top

J. 日期与时间
来源：http://pez.aibaodan.cn

================================================================================
来源：http://zki.ivvv.top

[J01] 获取当前时间
来源：http://ndd.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ybn.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vkq.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://rhz.yj202588.top

TS:   new Date();  Date.now()
来源：http://htv.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qeh.tian-w.cn

Go:   time.Now()
来源：http://kai.cqqwz.cn

Ruby: Time.now
来源：http://pyq.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mpt.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://veq.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hic.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kgf.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kze.yfazqb.com

TS:   d.toISOString()
来源：http://lwq.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://onf.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mzu.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nde.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nso.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://sje.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lpn.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fex.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://eey.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://xig.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jql.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cvh.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://mfk.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ncu.smart0.xyz

[J04] 时间戳与日期互转
来源：http://bup.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xfp.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nph.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cwq.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tzl.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jar.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://drn.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mjk.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jkt.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://qrh.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://hif.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gpp.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzr.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://olz.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://kjw.shangyingyoupin.top


<!-- 参考信息 -->