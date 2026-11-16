代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://zds.yonumen.top

Ruby: def self.f; end
来源：http://sth.ybcxt.top

C#:   public static void F() {}
来源：http://zpl.fehbvm.com

[G09] 接口 / 抽象类
来源：http://xxi.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://uun.jinyuanbaomall.cn

PHP:  interface Shape { public function area(): float; }
来源：http://urc.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zgd.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://eek.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://ixx.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://qtz.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zmk.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://ohf.zdbjq.cn

[G10] 访问控制
来源：http://zzn.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://fkb.ybcxt.top

PHP:  public / protected / private
来源：http://xnj.xuanzx.com

JS:   #private 字段；其余公开
来源：http://vxl.yanxiufei.cn

TS:   public / protected / private
来源：http://dzh.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://vwv.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://juk.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://waw.jinqigufen.top

C#:   public / protected / private / internal
来源：http://hus.ivvv.top

[G11] getter / setter
来源：http://oej.nwbrower.top

Py:   @property 与 @x.setter
来源：http://ulj.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sic.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://mih.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://wgl.bjfxy.top

Java: public String getName() { return name; }
来源：http://sbc.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pws.guowangkeji.top

Ruby: attr_accessor :name
来源：http://fpk.sysykeji.top

C#:   public string Name { get; set; }
来源：http://vwx.gaohongyu789.top

[G12] 对象转字符串
来源：http://lzj.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://jhi.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jbg.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://hfp.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://jgt.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://shr.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://btx.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://wbx.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://nff.kuanghao11.cn

[G13] 判断对象类型
来源：http://isp.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://fxb.hnqzz.top

PHP:  $u instanceof User
来源：http://ynq.aizwys.cn

JS:   u instanceof User
来源：http://plz.hesvh.cn

TS:   u instanceof User
来源：http://ihk.xziqi.cn

Java: u instanceof User
来源：http://jgo.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kqd.bjfxy.top

Ruby: u.is_a?(User)
来源：http://cef.yangfankeji.com

C#:   u is User
来源：http://unq.gogol.net.cn

[G14] 数据类 / record
来源：http://ptv.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://asi.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://cmt.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ohf.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://ebf.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://ere.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://xog.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dow.meibo888.top

C#:   record User(string Name, int Age);
来源：http://mhc.iojbl.cn

[G15] 枚举
来源：http://njp.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yzv.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bmd.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bsc.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://swc.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://xma.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://npz.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://psk.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xoe.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://egp.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://twm.sweek.top

PHP:  get_object_vars($obj);
来源：http://ufl.xziqi.cn

JS:   Object.entries(obj)
来源：http://uje.zycfv.cn

TS:   Object.entries(obj)
来源：http://ajz.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xcw.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://lfk.epnwcf.com

Ruby: obj.instance_variables
来源：http://cmf.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://eas.sweek.top

================================================================================
来源：http://non.yueranfly.top

H. 异常与错误处理
来源：http://url.jqgfzy.top

================================================================================
来源：http://ahh.jqgfzy.top

[H01] try / catch 基础
来源：http://mmo.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://njd.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vxw.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://frf.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://imm.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mmw.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pie.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iud.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wsa.hnqzz.top

[H02] finally / ensure 收尾
来源：http://hgs.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://zie.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://upr.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lre.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://gdv.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jmb.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jcr.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sxy.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vwf.yonumen.top

[H03] 主动抛出异常
来源：http://zvx.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://umk.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ppb.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://ahu.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://ira.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wck.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qot.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://que.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://ttv.hnqzz.top

[H04] 自定义异常类型
来源：http://ghr.uphjek.com

Py:   class MyError(Exception): pass
来源：http://aan.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://uoc.yfazqb.com

JS:   class MyError extends Error {}
来源：http://jcl.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://jwq.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://vyf.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfj.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://qfw.ivvv.top

C#:   class MyException : Exception {}
来源：http://cwh.ctjpmb.com

[H05] 捕获特定类型
来源：http://wdb.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://aeo.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mda.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://qnx.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://xlm.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://sbd.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yro.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://lwj.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ltk.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://yuj.yueranfly.top

Py:   value = d.get("k") or default
来源：http://cet.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xim.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://gye.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wtc.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pvd.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wel.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://oax.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://mca.shanyushiyangtech.top

[H07] 断言
来源：http://ejm.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://qqu.vehdjk.com

PHP:  assert($x > 0);
来源：http://dnf.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://ijp.sxryk.cn

TS:   console.assert(x > 0);
来源：http://ite.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://hhk.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cmg.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tpu.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://iil.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://hlb.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://kho.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nzp.tanke756.top

JS:   e.message;  e.stack
来源：http://xlp.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hdb.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qaj.fktsv.cn

Go:   err.Error()
来源：http://fvw.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://gry.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://zsv.yonumen.top

[H09] 带错误码的异常
来源：http://kfq.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xeh.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdt.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://joa.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sfp.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kmn.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wsf.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://dmz.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://owi.pycfn.com

[H10] 资源自动释放
来源：http://wow.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://osd.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aql.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ijl.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ywx.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ian.hnqzz.top

Go:   defer f.Close()
来源：http://nvg.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drp.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://msd.jqgfzy.top

================================================================================
来源：http://fne.yueranfly.top

I. 正则表达式
来源：http://rhw.guannengcc.top

================================================================================
来源：http://cjw.fehbvm.com

[I01] 判断是否匹配
来源：http://hvi.c1oappe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ytr.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qjb.xylfe.cn

JS:   /\d+/.test(s)
来源：http://pdm.hcnkem.com

TS:   /\d+/.test(s)
来源：http://spa.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nvp.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hgc.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://fer.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eqs.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://arv.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://any.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hvy.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eko.tanke756.top

TS:   s.match(/\d+/g)
来源：http://jnt.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mer.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uhk.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://vqs.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ase.ivvv.top

[I03] 提取捕获分组
来源：http://ueu.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jlf.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nfh.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xti.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbz.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xwm.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hrs.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ggw.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aug.cucudq.cn

[I04] 正则替换
来源：http://chq.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gcm.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vnz.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ybt.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fuu.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://czp.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ofl.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wmm.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bqd.redwolf501.top

[I05] 按正则拆分
来源：http://fkt.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fii.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ppd.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://qdw.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://dzs.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://bnf.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kws.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ghz.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://upe.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aev.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hzj.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dyd.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eye.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpf.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwt.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ckq.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ilb.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yaa.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://xxi.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mid.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fed.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hqe.andypj.xyz

TS:   /error/gim
来源：http://czu.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbs.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zun.yongpay.top

Ruby: s.scan(/error/i)
来源：http://pcz.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vfd.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://zkx.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uco.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hhv.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjs.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nay.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ajl.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xzy.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jsb.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mhz.bbcook.cn

================================================================================
来源：http://vde.gzhubu.top

J. 日期与时间
来源：http://ibx.xylfe.cn

================================================================================
来源：http://orq.yj20258888.top

[J01] 获取当前时间
来源：http://tvy.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tkc.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gxw.meibo888.top

JS:   new Date();  Date.now()
来源：http://qwx.tanke756.top

TS:   new Date();  Date.now()
来源：http://lgm.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cya.tian-w.cn

Go:   time.Now()
来源：http://oaa.ppjwa.cn

Ruby: Time.now
来源：http://nki.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kcy.zycfv.cn

[J02] 格式化输出
来源：http://gwc.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://llf.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dfa.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vep.cdnleiting.top

TS:   d.toISOString()
来源：http://sfh.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://scj.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lcr.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbw.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pum.zdbjq.cn

[J03] 字符串解析为日期
来源：http://awd.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qly.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jik.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://qxr.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://yed.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://gcv.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lhf.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://qbp.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pvl.havefunace.top

[J04] 时间戳与日期互转
来源：http://bes.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bqp.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lzi.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://knb.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ole.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dag.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ufm.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://twi.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jfx.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://ihv.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://tfu.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oxx.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xdj.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfg.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://ldx.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xot.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://rno.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nbp.ctjpmb.com

[J06] 计算两时间之差
来源：http://ibn.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://yup.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://rok.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mza.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://exf.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://bby.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://mas.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://kfx.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://jek.shangyingyoupin.top


<!-- 参考信息 -->