代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://psd.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://scu.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://obh.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://fmo.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://ply.birdmap.top

[G07] 调用父类方法
来源：http://dpx.bjfxy.top

Py:   super().greet()
来源：http://qks.zhongyouzk.top

PHP:  parent::greet();
来源：http://ykl.shanyushiyangkeji.top

JS:   super.greet();
来源：http://gce.shzxlz.cn

TS:   super.greet();
来源：http://zev.zdbjq.cn

Java: super.greet();
来源：http://gdg.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jtm.kuanghao11.cn

Ruby: super
来源：http://qbb.daxiang520.top

C#:   base.Greet();
来源：http://gnc.pycfn.com

[G08] 静态方法与属性
来源：http://dzx.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://diz.hnqzz.top

PHP:  public static function f() {}
来源：http://bre.sjlbkw.cn

JS:   static f() {}
来源：http://efz.hongshengwenyu.top

TS:   static f(): void {}
来源：http://zjb.havefunace.top

Java: static void f() {}
来源：http://gxj.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://alo.epnwcf.com

Ruby: def self.f; end
来源：http://hwd.uphjek.com

C#:   public static void F() {}
来源：http://qat.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://sfa.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://ugs.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://lkw.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://lqq.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://fxp.hcnkem.com

Java: interface Shape { double area(); }
来源：http://ebp.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://aey.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://keq.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://cpp.zhixingplan.top

[G10] 访问控制
来源：http://mwn.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://qud.ppjwa.cn

PHP:  public / protected / private
来源：http://omw.mhx1999.top

JS:   #private 字段；其余公开
来源：http://jni.jiagoushi.top

TS:   public / protected / private
来源：http://hqg.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://kiu.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qsi.hywenlv.cn

Ruby: public / protected / private
来源：http://xza.epnwcf.com

C#:   public / protected / private / internal
来源：http://jws.birdmap.top

[G11] getter / setter
来源：http://obp.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://qjn.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rac.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://ixx.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://ufk.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://ifq.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rbs.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://lgx.c1oappe.top

C#:   public string Name { get; set; }
来源：http://hbh.c1oappe.top

[G12] 对象转字符串
来源：http://cog.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://sqc.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kzk.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://oza.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://gof.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://ttz.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tpv.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://ycy.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://alo.mhx1999.top

[G13] 判断对象类型
来源：http://xgf.kuanghao11.cn

Py:   isinstance(u, User)
来源：http://pcr.havefunace.top

PHP:  $u instanceof User
来源：http://kao.nwbrower.top

JS:   u instanceof User
来源：http://kkz.meibo888.top

TS:   u instanceof User
来源：http://mdc.xziqi.cn

Java: u instanceof User
来源：http://iqk.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fxu.tian-w.cn

Ruby: u.is_a?(User)
来源：http://ayh.hywenlv.cn

C#:   u is User
来源：http://iku.xziqi.cn

[G14] 数据类 / record
来源：http://vxh.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kmd.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ahj.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://vge.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://ujp.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://ahw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://utk.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qxk.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://wcg.uphjek.com

[G15] 枚举
来源：http://zwv.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xft.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pqx.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xab.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cnf.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://nqf.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgf.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://vxy.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tts.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://vae.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nor.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://sve.hcnkem.com

JS:   Object.entries(obj)
来源：http://pqw.yongpay.top

TS:   Object.entries(obj)
来源：http://rrj.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oso.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://phh.vehdjk.com

Ruby: obj.instance_variables
来源：http://quy.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://jvt.hcnkem.com

================================================================================
来源：http://kpp.shuidangran.top

H. 异常与错误处理
来源：http://jlu.gotoacloud.top

================================================================================
来源：http://sek.zycfv.cn

[H01] try / catch 基础
来源：http://bkn.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hsw.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rvq.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rse.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dso.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pnt.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oyy.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jca.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cut.bjfxy.top

[H02] finally / ensure 收尾
来源：http://wji.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vss.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://stc.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://svh.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ygk.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://cuw.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hry.52xcode.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gsx.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rnq.zhoulong.xyz

[H03] 主动抛出异常
来源：http://kvs.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://ita.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ngc.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://zui.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://uwv.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ccr.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fso.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aoi.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://pce.gaohongyu789.top

[H04] 自定义异常类型
来源：http://soq.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://ffi.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://lcn.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://hgu.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://tli.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://mxh.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sbg.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://url.cheryme.top

C#:   class MyException : Exception {}
来源：http://hor.jinqigufen.top

[H05] 捕获特定类型
来源：http://sjo.zdbjq.cn

Py:   except ValueError as e:
来源：http://cev.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://edv.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://doh.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://lmh.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://mdg.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hkz.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://jic.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gxf.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://upp.tanke756.top

Py:   value = d.get("k") or default
来源：http://tzl.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iev.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xll.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://rxi.yonumen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wuu.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rou.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://pje.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://igz.uphjek.com

[H07] 断言
来源：http://dob.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://vlw.snrcjt.cn

PHP:  assert($x > 0);
来源：http://mkn.pycfn.com

JS:   console.assert(x > 0);
来源：http://abp.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://gxp.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://cld.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qjb.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://unj.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://akw.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://dzw.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://ccs.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fec.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://hhw.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ddf.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://aiz.ybcxt.top

Go:   err.Error()
来源：http://tgy.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://pwv.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://stx.daxiang520.top

[H09] 带错误码的异常
来源：http://ytd.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sxu.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xff.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://suo.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fkn.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uyc.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vlt.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://klk.fanxiaobao.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://njg.wangdashe.top

[H10] 资源自动释放
来源：http://qit.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zxt.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iha.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jaz.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kdy.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nbd.fengsongda.top

Go:   defer f.Close()
来源：http://udw.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dlo.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ual.shuidangran.top

================================================================================
来源：http://goh.cdnleiting.top

I. 正则表达式
来源：http://hhm.nanxinkj.top

================================================================================
来源：http://ete.0kj1m.cn

[I01] 判断是否匹配
来源：http://ddg.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eoe.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://fyy.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://wur.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://nia.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cuu.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dcq.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://rhe.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wnz.yangfankeji.com

[I02] 提取所有匹配
来源：http://fjp.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://shw.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vse.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dhd.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://abs.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kwy.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://avz.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://nsj.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eic.iojbl.cn

[I03] 提取捕获分组
来源：http://djf.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://heg.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpd.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ywu.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aou.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://asf.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://phz.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bgc.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://phc.ydjk.org.cn

[I04] 正则替换
来源：http://zvm.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wje.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rls.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kbb.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hle.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nfo.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://shw.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hhi.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zss.cqqwz.cn

[I05] 按正则拆分
来源：http://dxf.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hdf.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yra.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://xhf.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://lov.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://cdf.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://acn.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://skz.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kzk.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://arg.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxp.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lux.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iss.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zob.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nnp.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bkd.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sbl.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://krn.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://bsg.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bix.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cmz.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zln.52xcode.cn

TS:   /error/gim
来源：http://onq.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://czn.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nwr.birdmap.top

Ruby: s.scan(/error/i)
来源：http://xpv.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qrl.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://oyl.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bof.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hob.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://efz.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlx.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dhb.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rwv.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://abu.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lqc.chenlongwang.top

================================================================================
来源：http://bco.svipenyu.cn

J. 日期与时间
来源：http://sfr.hfpthk.cn

================================================================================
来源：http://mxm.guowangkeji.top

[J01] 获取当前时间
来源：http://yyc.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mpa.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgf.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://iom.yvedp.cn

TS:   new Date();  Date.now()
来源：http://wta.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pym.ywan-chungtsiang.top

Go:   time.Now()
来源：http://wip.quarkkingdee.top

Ruby: Time.now
来源：http://ypj.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://agk.hnxiangtu.top

[J02] 格式化输出
来源：http://jni.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://roh.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hkc.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ixg.hfpthk.cn

TS:   d.toISOString()
来源：http://lof.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://svr.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yel.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ewc.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vmx.smart0.xyz

[J03] 字符串解析为日期
来源：http://lcg.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xdx.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lsv.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://kqm.havefunace.top

TS:   new Date("2024-01-02")
来源：http://vne.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://die.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rgz.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://nqe.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xdi.xylfe.cn

[J04] 时间戳与日期互转
来源：http://tzz.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pfw.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aee.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dcp.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://rmp.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exw.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hls.yongpay.top


<!-- 参考信息 -->