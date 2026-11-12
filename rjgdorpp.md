代发 wailian999

[G06] 重写方法
来源：http://wwf.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://qsl.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fla.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://hzp.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://wyj.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://lit.cheryme.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kiv.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://vya.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://kzb.yuxming.cn

[G07] 调用父类方法
来源：http://wmd.nwbrower.top

Py:   super().greet()
来源：http://rrd.shangyingyoupin.top

PHP:  parent::greet();
来源：http://jzt.nwbrower.top

JS:   super.greet();
来源：http://ikv.vqdsnc.cn

TS:   super.greet();
来源：http://vgf.snrcjt.cn

Java: super.greet();
来源：http://mbo.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pni.gogol.net.cn

Ruby: super
来源：http://dkh.dianchejie.cn

C#:   base.Greet();
来源：http://zdr.cdnleiting.top

[G08] 静态方法与属性
来源：http://wxm.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://swc.hnxiangtu.top

PHP:  public static function f() {}
来源：http://vhb.sufxvd.cn

JS:   static f() {}
来源：http://woa.guowangkeji.top

TS:   static f(): void {}
来源：http://txp.wangshuangyany.cn

Java: static void f() {}
来源：http://lix.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://cou.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://ueo.ydzc1.top

C#:   public static void F() {}
来源：http://tbq.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://zav.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://gvc.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wql.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ulx.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://nqb.xziqi.cn

Java: interface Shape { double area(); }
来源：http://jmb.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://vtm.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sdd.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://jdi.fzhhl.top

[G10] 访问控制
来源：http://ufx.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://dpn.sufxvd.cn

PHP:  public / protected / private
来源：http://jyx.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://uzu.zhixingplan.top

TS:   public / protected / private
来源：http://kbd.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://hat.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://arb.yangfankeji.com

Ruby: public / protected / private
来源：http://zsn.epnwcf.com

C#:   public / protected / private / internal
来源：http://zep.ctjpmb.com

[G11] getter / setter
来源：http://wfc.epnwcf.com

Py:   @property 与 @x.setter
来源：http://fbz.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://pnl.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://itu.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://mdi.hesvh.cn

Java: public String getName() { return name; }
来源：http://oif.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mrc.yuanzhike.top

Ruby: attr_accessor :name
来源：http://lpi.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://rve.ctjpmb.com

[G12] 对象转字符串
来源：http://mjw.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://mmv.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ujw.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://swo.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://amx.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://and.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://csq.cucudq.cn

Ruby: def to_s; @name; end
来源：http://zye.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://qpf.gzhubu.top

[G13] 判断对象类型
来源：http://cch.hcnkem.com

Py:   isinstance(u, User)
来源：http://odm.cashguo.top

PHP:  $u instanceof User
来源：http://qwp.hysaishi.cn

JS:   u instanceof User
来源：http://lgg.nanxuanxn.top

TS:   u instanceof User
来源：http://mic.shanyushiyangkeji.top

Java: u instanceof User
来源：http://jvh.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vna.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://nyi.yj202588.top

C#:   u is User
来源：http://twg.tianlin.xyz

[G14] 数据类 / record
来源：http://cgn.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uda.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://jvd.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://sgg.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://aby.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://kls.mhx1999.top

Go:   type User struct { Name string; Age int }
来源：http://fhp.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://izq.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://tmd.yueranfly.top

[G15] 枚举
来源：http://srs.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://imb.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jgj.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wev.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fmq.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://vsa.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dof.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://rdl.bbcook.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://evr.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://flg.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hus.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://omx.ybcxt.top

JS:   Object.entries(obj)
来源：http://djj.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ezr.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wpj.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zas.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://xss.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://bcc.dianchejie.cn

================================================================================
来源：http://skb.sweek.top

H. 异常与错误处理
来源：http://fji.ctjpmb.com

================================================================================
来源：http://zjl.bjfxy.top

[H01] try / catch 基础
来源：http://nhy.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jqw.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ftt.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wdt.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fyn.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lcy.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wiy.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://avv.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dqr.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://jim.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kma.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://vug.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fbf.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gsj.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://miu.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ohw.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vnn.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zmw.316326.xyz

[H03] 主动抛出异常
来源：http://xok.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://gjw.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lch.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://xzn.ywan-chungtsiang.top

TS:   throw new Error("错误信息");
来源：http://zlz.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yti.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ecl.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://tjj.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sdl.xziqi.cn

[H04] 自定义异常类型
来源：http://rqw.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://ymg.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://gba.mhx1999.top

JS:   class MyError extends Error {}
来源：http://gmc.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://szm.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://kaz.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yph.sufxvd.cn

Ruby: class MyError < StandardError; end
来源：http://gxj.nwbrower.top

C#:   class MyException : Exception {}
来源：http://xmj.sxryk.cn

[H05] 捕获特定类型
来源：http://czs.jyoumei.cn

Py:   except ValueError as e:
来源：http://xtv.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pex.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://nfd.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://bfi.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://acv.ydzc1.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fhc.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ogk.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oxb.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://mra.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://sda.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://ckf.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ktj.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://mbg.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wfy.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gsc.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://ibr.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://ivw.dashuyun.cn

[H07] 断言
来源：http://knb.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://wna.yueranfly.top

PHP:  assert($x > 0);
来源：http://uqp.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://qiy.nanxinkj.top

TS:   console.assert(x > 0);
来源：http://sbv.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://rse.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vpo.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://cgp.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://qfq.hnqzz.top

[H08] 获取错误信息与堆栈
来源：http://wmh.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://qgy.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rhz.andypj.xyz

JS:   e.message;  e.stack
来源：http://iqp.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yfj.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://uhu.52xcode.cn

Go:   err.Error()
来源：http://mwp.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://ptg.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://sux.bbcook.cn

[H09] 带错误码的异常
来源：http://vqf.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zjl.zdqjudy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ovj.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://chw.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hfc.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwt.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kox.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rda.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://zbj.zhoulong.xyz

[H10] 资源自动释放
来源：http://wqi.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cce.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iwi.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qkm.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pcl.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nre.hcnkem.com

Go:   defer f.Close()
来源：http://ilj.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hmo.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dhl.zdqjudy.top

================================================================================
来源：http://utj.yangfankeji.com

I. 正则表达式
来源：http://cfx.cheryme.top

================================================================================
来源：http://irh.birdmap.top

[I01] 判断是否匹配
来源：http://bcs.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ecy.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://whu.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://bkg.zycfv.cn

TS:   /\d+/.test(s)
来源：http://tzn.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qel.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xhb.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://xdq.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://srp.kuanghao11.cn

[I02] 提取所有匹配
来源：http://cgd.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://yhj.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fqf.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mzr.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://shc.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bjf.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cmu.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://lld.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbn.316326.xyz

[I03] 提取捕获分组
来源：http://sxp.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ypt.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zkl.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xxj.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nee.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://coo.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eny.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xyp.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nvd.fanxiaobao.xyz

[I04] 正则替换
来源：http://asx.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nxc.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uen.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ble.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://knk.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xyo.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dnf.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tvi.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hpe.316326.xyz

[I05] 按正则拆分
来源：http://dib.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wuj.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdm.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://uxt.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://fnl.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://bru.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oxo.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://owr.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lzc.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nqz.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ihy.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://adp.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://igp.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pva.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aig.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sls.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fye.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ffu.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://jzj.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dnj.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyy.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://opw.fktsv.cn

TS:   /error/gim
来源：http://gvv.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sbo.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hjv.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://bsh.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nwh.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://gsk.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tir.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gns.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxa.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wer.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hwe.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sgw.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gnc.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bqq.jinqigufen.top

================================================================================
来源：http://muu.ydjk.org.cn

J. 日期与时间
来源：http://cxf.jianghu66.top

================================================================================
来源：http://ifq.316326.xyz

[J01] 获取当前时间
来源：http://pru.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pvw.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nis.mhx1999.top

JS:   new Date();  Date.now()
来源：http://qmy.xylfe.cn

TS:   new Date();  Date.now()
来源：http://bdz.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tay.yueranfly.top

Go:   time.Now()
来源：http://xqx.snrcjt.cn

Ruby: Time.now
来源：http://yog.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wkf.snrcjt.cn

[J02] 格式化输出
来源：http://avf.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ghc.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boz.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pbb.xuanzx.com

TS:   d.toISOString()
来源：http://rgl.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ipx.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cln.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://umk.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://feg.tarul.cn

[J03] 字符串解析为日期
来源：http://vue.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vhz.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yto.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://jwv.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://uon.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rwu.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://czu.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://zmp.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qda.daxiang520.top

[J04] 时间戳与日期互转
来源：http://iks.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://viw.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://spz.meibo888.top


<!-- 参考信息 -->