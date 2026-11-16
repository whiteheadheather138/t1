代发 wailian999

PHP:  public static function f() {}
来源：http://umr.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://osa.cheryme.top

TS:   static f(): void {}
来源：http://zob.dianchejie.cn

Java: static void f() {}
来源：http://kie.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://euh.xylfe.cn

Ruby: def self.f; end
来源：http://zuw.yj20258888.top

C#:   public static void F() {}
来源：http://dnl.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://twq.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://ioe.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://ilz.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://yxd.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://wxz.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://zgy.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://tvc.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://emt.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://ndu.smart0.xyz

[G10] 访问控制
来源：http://uri.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qlp.ydzc1.top

PHP:  public / protected / private
来源：http://yys.yj20258888.top

JS:   #private 字段；其余公开
来源：http://jpd.fanxiaobao.xyz

TS:   public / protected / private
来源：http://hau.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://hte.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ive.xziqi.cn

Ruby: public / protected / private
来源：http://qwh.svipenyu.cn

C#:   public / protected / private / internal
来源：http://gyw.cucudq.cn

[G11] getter / setter
来源：http://uhi.tanke756.top

Py:   @property 与 @x.setter
来源：http://iij.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vcd.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://tyr.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://tyt.fengsongda.top

Java: public String getName() { return name; }
来源：http://bmr.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ajm.yj20258.top

Ruby: attr_accessor :name
来源：http://kxv.jianghu66.top

C#:   public string Name { get; set; }
来源：http://qri.jinqigufen.top

[G12] 对象转字符串
来源：http://kyz.birdmap.top

Py:   def __str__(self): return self.name
来源：http://iwk.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://sqa.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://ulb.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://htf.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://awk.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://blm.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://kmm.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://abw.haohaochexian.top

[G13] 判断对象类型
来源：http://gws.hysaishi.cn

Py:   isinstance(u, User)
来源：http://wbw.dianchejie.cn

PHP:  $u instanceof User
来源：http://sci.yuanzhike.top

JS:   u instanceof User
来源：http://dxc.shangyingyoupin.top

TS:   u instanceof User
来源：http://dul.meibo888.top

Java: u instanceof User
来源：http://aei.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mpg.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://noe.smart0.xyz

C#:   u is User
来源：http://fac.cheryme.top

[G14] 数据类 / record
来源：http://evy.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xzf.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://ows.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://uou.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://mvc.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://muc.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://jhn.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bvn.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://iyb.jinqigufen.top

[G15] 枚举
来源：http://awx.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uvt.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jij.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lst.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qml.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://lxr.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ofd.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://xyl.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tur.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://dil.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tsu.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://anx.yonumen.top

JS:   Object.entries(obj)
来源：http://uei.yuanzhike.top

TS:   Object.entries(obj)
来源：http://jvd.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qti.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pwb.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://hra.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://nsj.ctjpmb.com

================================================================================
来源：http://uub.dashuyun.cn

H. 异常与错误处理
来源：http://ldf.uphjek.com

================================================================================
来源：http://klm.sweek.top

[H01] try / catch 基础
来源：http://xgo.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jqk.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hcn.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lbl.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eyb.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxk.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wzi.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jsw.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hiv.cashguo.top

[H02] finally / ensure 收尾
来源：http://vxb.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://mnr.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://qcr.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://uzt.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://skg.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qbe.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://fgx.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bnx.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://khj.snrcjt.cn

[H03] 主动抛出异常
来源：http://wbt.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://kzq.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eoq.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://fsn.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://orz.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rwl.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://whq.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iks.jinqigufen.top

C#:   throw new ArgumentException("错误信息");
来源：http://nft.xinyue.icu

[H04] 自定义异常类型
来源：http://xmi.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://xmc.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://vbk.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://svt.sxryk.cn

TS:   class MyError extends Error {}
来源：http://mjw.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://voy.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gfi.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://zff.xylfe.cn

C#:   class MyException : Exception {}
来源：http://xvx.chenlongwang.top

[H05] 捕获特定类型
来源：http://rzb.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://unn.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aft.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://cvm.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://buh.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://yxm.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://for.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://zdr.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gdj.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://ano.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://pks.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://uhe.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xyg.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://nod.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pjl.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rbh.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://pbg.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://rqu.ctjpmb.com

[H07] 断言
来源：http://eth.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://pnq.sysykeji.top

PHP:  assert($x > 0);
来源：http://dtf.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://cqe.jianghu66.top

TS:   console.assert(x > 0);
来源：http://fdq.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://qgt.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lis.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vwu.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://hqk.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://vyx.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://yvu.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jcq.yonumen.top

JS:   e.message;  e.stack
来源：http://zev.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mxc.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jns.shanyushiyangkeji.top

Go:   err.Error()
来源：http://jua.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://ydz.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://slo.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://kkl.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpf.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nvo.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nvt.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ihd.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://reh.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xbq.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://utg.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wou.xinyue.icu

[H10] 资源自动释放
来源：http://ncf.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxk.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phr.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ttg.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mhx.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ujj.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://crr.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fjl.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dkp.jiagoushi.top

================================================================================
来源：http://aqs.jianghu66.top

I. 正则表达式
来源：http://tzp.shanyushiyangtech.top

================================================================================
来源：http://lvb.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://qda.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcn.jlsjyb.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fdq.bbcook.cn

JS:   /\d+/.test(s)
来源：http://uoz.ydzc1.top

TS:   /\d+/.test(s)
来源：http://qhg.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lpw.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ghn.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://wdi.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gju.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://cmh.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://gii.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyp.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qdf.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://vyf.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fkl.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dvv.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://btd.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vkb.andypj.xyz

[I03] 提取捕获分组
来源：http://lun.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lqt.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aem.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mds.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://puy.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oax.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://arl.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ori.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qat.gogol.net.cn

[I04] 正则替换
来源：http://sst.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ukw.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tvk.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://rte.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://bgc.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://icy.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bae.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mfr.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jzj.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://rzd.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yaw.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aui.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://bnu.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://gaa.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://cgv.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jji.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bph.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ole.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wri.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vni.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ruj.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ggt.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bzw.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tpe.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mto.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bec.gzhubu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://exr.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://lpc.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zvz.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ubc.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tic.fengsongda.top

TS:   /error/gim
来源：http://tti.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://muw.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ngq.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://kgs.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lig.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://gdk.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrz.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jyx.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bcx.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oxd.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://frm.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ody.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gku.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dfy.yangfankeji.com

================================================================================
来源：http://yil.zhaomingkeji.xyz

J. 日期与时间
来源：http://aay.chenzaomai.com

================================================================================
来源：http://bch.gotoacloud.top

[J01] 获取当前时间
来源：http://xvw.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fyz.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qvz.yongpay.top

JS:   new Date();  Date.now()
来源：http://xxo.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://jnt.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jdp.gaohongyu789.top

Go:   time.Now()
来源：http://hls.dashuyun.cn

Ruby: Time.now
来源：http://rxj.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xeu.bbcook.cn

[J02] 格式化输出
来源：http://ssa.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cvx.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://znl.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iet.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://gmb.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://peb.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yak.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://imw.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ncw.yangfankeji.com

[J03] 字符串解析为日期
来源：http://gph.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rjd.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tsl.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://evh.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://vhr.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://zof.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vro.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://bei.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zrm.yj20258888.top

[J04] 时间戳与日期互转
来源：http://roh.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wrb.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qbk.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nzh.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lgk.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hal.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qol.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://czu.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yph.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://qmm.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://jtf.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lbn.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cha.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xcl.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://hyi.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sio.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://kuv.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hno.daria6918.cn

[J06] 计算两时间之差
来源：http://yud.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://sxn.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://tqb.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hje.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sec.zhijiandao.cn


<!-- 参考信息 -->