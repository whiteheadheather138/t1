代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ifo.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://cjc.ydjk.org.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dkp.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://lnr.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://bzb.tanke756.top

[G07] 调用父类方法
来源：http://yni.dianchejie.cn

Py:   super().greet()
来源：http://dqp.ivvv.top

PHP:  parent::greet();
来源：http://swy.pengpengdd.cyou

JS:   super.greet();
来源：http://mto.chenjidiqi.icu

TS:   super.greet();
来源：http://jzj.ydjk.org.cn

Java: super.greet();
来源：http://xmy.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mgh.zhijiandao.cn

Ruby: super
来源：http://eys.316326.xyz

C#:   base.Greet();
来源：http://ymq.jqgfzy.top

[G08] 静态方法与属性
来源：http://mxy.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwi.9152youxi.cn

PHP:  public static function f() {}
来源：http://rmz.chenzaomai.com

JS:   static f() {}
来源：http://obf.jiagoushi.top

TS:   static f(): void {}
来源：http://gei.hcnkem.com

Java: static void f() {}
来源：http://hqo.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hvm.pycfn.com

Ruby: def self.f; end
来源：http://nzk.chenlongwang.top

C#:   public static void F() {}
来源：http://bab.yvedp.cn

[G09] 接口 / 抽象类
来源：http://ets.smart0.xyz

Py:   from abc import ABC, abstractmethod
来源：http://hrh.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://zry.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oqb.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://riu.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://xpq.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://del.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aeg.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://lpz.iojbl.cn

[G10] 访问控制
来源：http://iar.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://max.jqgfzy.top

PHP:  public / protected / private
来源：http://wlw.vehdjk.com

JS:   #private 字段；其余公开
来源：http://wtw.fehbvm.com

TS:   public / protected / private
来源：http://fxp.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://qud.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dhs.mhx1999.top

Ruby: public / protected / private
来源：http://sag.tianlin.xyz

C#:   public / protected / private / internal
来源：http://oka.yj20258888.top

[G11] getter / setter
来源：http://tvj.zhiwuduotai.top

Py:   @property 与 @x.setter
来源：http://eti.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bwa.316326.xyz

JS:   get name() { return this._name; }
来源：http://svh.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://tar.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://ewn.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://dwc.zhengqikj.top

Ruby: attr_accessor :name
来源：http://cut.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://wki.zhongyouzk.top

[G12] 对象转字符串
来源：http://wie.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://gad.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fit.hammf.cn

JS:   toString() { return this.name; }
来源：http://rfv.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://asd.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://ail.yj202588.top

Go:   func (u User) String() string { return u.Name }
来源：http://htp.tanke756.top

Ruby: def to_s; @name; end
来源：http://bal.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://una.ehwqpu.com

[G13] 判断对象类型
来源：http://fsc.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://tqs.cheryme.top

PHP:  $u instanceof User
来源：http://gpu.iojbl.cn

JS:   u instanceof User
来源：http://fgv.jinghuilouyu.cn

TS:   u instanceof User
来源：http://ioo.chenzaomai.com

Java: u instanceof User
来源：http://xgd.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ale.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://urx.jiagoushi.top

C#:   u is User
来源：http://mxv.wangshuangyany.cn

[G14] 数据类 / record
来源：http://okf.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cik.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://hpy.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://mkg.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://iwe.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://eie.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://aam.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qep.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://irn.svipenyu.cn

[G15] 枚举
来源：http://kup.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://plt.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://drv.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dzv.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tef.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://xyu.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://spy.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://uba.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fwf.cheryme.top

[G16] 对象转数组 / 字典
来源：http://cix.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jcw.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://fqs.yj20258.top

JS:   Object.entries(obj)
来源：http://rgq.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://fpe.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nxm.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lig.nanxinkj.top

Ruby: obj.instance_variables
来源：http://zmh.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://njy.fanxiaobao.xyz

================================================================================
来源：http://ayc.tanke756.top

H. 异常与错误处理
来源：http://lgi.yj20258.top

================================================================================
来源：http://qeo.aizwys.cn

[H01] try / catch 基础
来源：http://jjs.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cas.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uhj.daxiang520.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ctr.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://siz.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yaw.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfg.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lwb.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kpw.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://wln.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://osn.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://goe.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nke.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://odm.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://lzg.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hgt.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://oic.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qpi.sweek.top

[H03] 主动抛出异常
来源：http://bcr.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://smb.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ubm.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://qri.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://nkk.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lkh.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ggd.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://efq.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://uyh.yongpay.top

[H04] 自定义异常类型
来源：http://oze.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://bab.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://zlv.uphjek.com

JS:   class MyError extends Error {}
来源：http://jtm.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://atd.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://pxj.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://odl.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://pog.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://nob.ppjwa.cn

[H05] 捕获特定类型
来源：http://ppy.zdqjudy.top

Py:   except ValueError as e:
来源：http://ntw.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rci.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://mbz.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://mad.shuidangran.top

Java: catch (IOException | SQLException e) {}
来源：http://cmm.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yen.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://aja.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rvc.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://hpz.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://gkq.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://nyr.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ljh.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ntl.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iko.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oky.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://kia.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://ifm.feifeiyinyue.top

[H07] 断言
来源：http://rrq.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://jkx.yj202588.top

PHP:  assert($x > 0);
来源：http://brm.fzhhl.top

JS:   console.assert(x > 0);
来源：http://ddp.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://bnu.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://zem.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ice.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://trk.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://uxa.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://gzc.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://bwy.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ltj.jiagoushi.top

JS:   e.message;  e.stack
来源：http://tkd.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://orn.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://prw.redwolf501.top

Go:   err.Error()
来源：http://umk.c1oappe.top

Ruby: e.message;  e.backtrace
来源：http://isj.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://ndg.vehdjk.com

[H09] 带错误码的异常
来源：http://kvr.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gux.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://qde.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jrj.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ddu.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pno.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://obo.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://xjl.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jib.meibo888.top

[H10] 资源自动释放
来源：http://fqa.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tpa.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mql.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vhv.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://apa.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://arb.ctjpmb.com

Go:   defer f.Close()
来源：http://ksu.9152youxi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lbi.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kve.shanyushiyangkeji.top

================================================================================
来源：http://iee.pycfn.com

I. 正则表达式
来源：http://sky.iojbl.cn

================================================================================
来源：http://sto.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://iut.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://csw.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cpx.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://vzm.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://yuc.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://noh.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mcp.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://ihv.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ttp.zhongyouzk.top

[I02] 提取所有匹配
来源：http://yjq.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://sud.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hsh.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ovg.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://wno.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rut.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fpz.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://uvl.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ryl.shzxlz.cn

[I03] 提取捕获分组
来源：http://cmo.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lkj.jinyuanbaomall.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jum.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hxj.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oee.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yhh.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ytl.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kga.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hom.quarkkingdee.top

[I04] 正则替换
来源：http://avt.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://dmv.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qbg.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://wsu.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://tem.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://ung.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://isw.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://xqo.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhk.tarul.cn

[I05] 按正则拆分
来源：http://niv.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ike.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://znn.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://imf.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://svg.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://ktp.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zyf.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://sea.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yxl.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nug.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://son.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://abs.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kxo.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://awg.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://guy.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mat.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cul.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hfx.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://xtp.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zcy.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hjy.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://znl.andypj.xyz

TS:   /error/gim
来源：http://awr.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dzo.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mql.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://bkx.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zyz.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://jhg.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mgi.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wkl.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xiu.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://seo.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://yil.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kmm.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ump.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fwp.uphjek.com

================================================================================
来源：http://xcm.zhixingplan.top

J. 日期与时间
来源：http://clk.fengsongda.top

================================================================================
来源：http://dys.jqgfzy.top

[J01] 获取当前时间
来源：http://rub.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ozx.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dsx.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://mxq.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://ezy.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dcu.chenzaomai.com

Go:   time.Now()
来源：http://pjr.fengsongda.top

Ruby: Time.now
来源：http://sgu.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xup.zhoulong.xyz

[J02] 格式化输出
来源：http://jwv.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgr.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yfr.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iic.kuanghao11.cn

TS:   d.toISOString()
来源：http://nxh.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vcp.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zkn.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dba.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://afz.zdqjudy.top

[J03] 字符串解析为日期
来源：http://kwe.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kqu.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ogr.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://eyx.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://vip.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://nyq.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jur.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://idl.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jnx.yonumen.top

[J04] 时间戳与日期互转
来源：http://vii.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sqz.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mcq.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iwd.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://amd.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvm.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vms.ydjk.org.cn


<!-- 参考信息 -->