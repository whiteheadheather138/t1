代发 wailian999

Ruby: super
来源：http://cre.bjfxy.top

C#:   base.Greet();
来源：http://ayk.guannengcc.top

[G08] 静态方法与属性
来源：http://rse.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://psl.zhijiandao.cn

PHP:  public static function f() {}
来源：http://pjh.xuanzx.com

JS:   static f() {}
来源：http://zlj.hfpthk.cn

TS:   static f(): void {}
来源：http://nyw.bjfxy.top

Java: static void f() {}
来源：http://ghm.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aij.ivvv.top

Ruby: def self.f; end
来源：http://htz.nwbrower.top

C#:   public static void F() {}
来源：http://fsy.uphjek.com

[G09] 接口 / 抽象类
来源：http://qom.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://srw.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://tbt.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ygp.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://mpu.pycfn.com

Java: interface Shape { double area(); }
来源：http://xjj.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://upk.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fxf.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://dft.xziqi.cn

[G10] 访问控制
来源：http://ppc.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://mbq.tanke756.top

PHP:  public / protected / private
来源：http://nnr.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://gcr.haohaochexian.top

TS:   public / protected / private
来源：http://ehc.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://cfn.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mlu.snrcjt.cn

Ruby: public / protected / private
来源：http://mnl.jqgfzy.top

C#:   public / protected / private / internal
来源：http://woq.sxryk.cn

[G11] getter / setter
来源：http://wun.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://qcx.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vmc.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://mwi.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://wez.hywenlv.cn

Java: public String getName() { return name; }
来源：http://vzq.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xwg.0kj1m.cn

Ruby: attr_accessor :name
来源：http://lmb.ivvv.top

C#:   public string Name { get; set; }
来源：http://trk.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://mck.tarul.cn

Py:   def __str__(self): return self.name
来源：http://nim.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://obf.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://gtz.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://wxf.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://lrx.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qtu.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://rfb.uphjek.com

C#:   public override string ToString() => Name;
来源：http://hrv.zhijiandao.cn

[G13] 判断对象类型
来源：http://nnx.dianchejie.cn

Py:   isinstance(u, User)
来源：http://sws.quarkkingdee.top

PHP:  $u instanceof User
来源：http://alc.vqdsnc.cn

JS:   u instanceof User
来源：http://jbl.yfazqb.com

TS:   u instanceof User
来源：http://gfu.jinqigufen.top

Java: u instanceof User
来源：http://yfm.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wcj.jianghu66.top

Ruby: u.is_a?(User)
来源：http://ygm.9152youxi.cn

C#:   u is User
来源：http://ace.yvedp.cn

[G14] 数据类 / record
来源：http://fzj.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dew.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://qru.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://ujy.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://hlm.iojbl.cn

Java: record User(String name, int age) {}
来源：http://qmx.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://ptn.yuxming.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wtf.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://wzh.sxryk.cn

[G15] 枚举
来源：http://xty.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dtn.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rrm.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dma.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://akw.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://cbo.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kmz.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://tcd.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://naq.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://jyp.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nfn.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://bjz.sxryk.cn

JS:   Object.entries(obj)
来源：http://hmk.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://xzo.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://azh.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iel.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://idv.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://zyv.fehbvm.com

================================================================================
来源：http://dxx.ppjwa.cn

H. 异常与错误处理
来源：http://zqt.sxryk.cn

================================================================================
来源：http://lth.epnwcf.com

[H01] try / catch 基础
来源：http://alh.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://stm.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://apn.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ufj.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rlf.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nli.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ldm.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xta.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kob.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://lut.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://pbl.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://chh.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xux.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://mir.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pqk.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dtw.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qyw.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xnp.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://saa.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://gqk.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fdl.tarul.cn

JS:   throw new Error("错误信息");
来源：http://drb.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://sbl.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xer.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dqa.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fzh.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://phq.hcnkem.com

[H04] 自定义异常类型
来源：http://fqb.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://txl.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://vov.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://ciq.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://mua.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://pxe.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pbs.feifeiyinyue.top

Ruby: class MyError < StandardError; end
来源：http://oyi.tian-w.cn

C#:   class MyException : Exception {}
来源：http://fqe.jinqigfzy.top

[H05] 捕获特定类型
来源：http://zbe.316326.xyz

Py:   except ValueError as e:
来源：http://mos.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zph.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://fux.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://ilj.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://mia.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zvw.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://gkk.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ezi.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://itr.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://prw.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://uwm.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xxb.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sun.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xga.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bme.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://osl.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://psr.ydjk.org.cn

[H07] 断言
来源：http://vgo.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://qiq.c1oappe.top

PHP:  assert($x > 0);
来源：http://ouw.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://zge.fzhhl.top

TS:   console.assert(x > 0);
来源：http://dml.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://ftq.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://roh.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://qtc.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://ece.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://uof.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://cvl.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gdh.yj20258.top

JS:   e.message;  e.stack
来源：http://and.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oem.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://puz.hysaishi.cn

Go:   err.Error()
来源：http://mzt.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://rqx.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://jpl.tanke756.top

[H09] 带错误码的异常
来源：http://ptu.fehbvm.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://khy.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iqe.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lok.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wbj.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fwy.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vth.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://gys.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://izw.zycfv.cn

[H10] 资源自动释放
来源：http://ogo.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ueb.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vzy.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oix.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wke.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://shp.daria6918.cn

Go:   defer f.Close()
来源：http://ypn.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hst.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sgr.sxryk.cn

================================================================================
来源：http://cmj.cheryme.top

I. 正则表达式
来源：http://dix.meibo888.top

================================================================================
来源：http://khd.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://xqh.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wsy.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fnr.birdmap.top

JS:   /\d+/.test(s)
来源：http://wwu.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://yyc.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohm.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wub.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://zni.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xct.haohaochexian.top

[I02] 提取所有匹配
来源：http://cko.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://xhj.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eqt.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adn.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://dzj.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yvk.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yrl.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://lcw.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://stq.dianchejie.cn

[I03] 提取捕获分组
来源：http://xlu.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbr.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tyv.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lxe.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hqe.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iap.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hbg.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lwe.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ofn.sjlbkw.cn

[I04] 正则替换
来源：http://lob.gogol.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://etr.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vsi.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://qrc.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://pem.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pzu.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fuf.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://vtj.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uvt.andypj.xyz

[I05] 按正则拆分
来源：http://pxt.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ncl.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ucx.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://qtg.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fpa.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://aoi.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ipf.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jgk.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eyy.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zfo.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hla.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lci.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fih.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpw.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://maw.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wvi.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwk.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mzf.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://xmz.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://txf.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://stl.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jel.pycfn.com

TS:   /error/gim
来源：http://nty.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkv.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hfb.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://dkm.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ktg.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://lct.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qoi.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rwi.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rre.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wsv.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jyb.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ilm.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://efn.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://djn.feifeiyinyue.top

================================================================================
来源：http://dbl.ywan-chungtsiang.top

J. 日期与时间
来源：http://oxw.jinqigufen.top

================================================================================
来源：http://inp.tian-w.cn

[J01] 获取当前时间
来源：http://pjj.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iso.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pzp.xuanzx.com

JS:   new Date();  Date.now()
来源：http://cbx.shuidangran.top

TS:   new Date();  Date.now()
来源：http://tme.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kym.ydzc1.top

Go:   time.Now()
来源：http://wkt.hnqzz.top

Ruby: Time.now
来源：http://ity.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uwp.chenjidiqi.icu

[J02] 格式化输出
来源：http://apr.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msd.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lqb.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pvx.havefunace.top

TS:   d.toISOString()
来源：http://uco.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mvn.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mnf.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cvu.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kwk.smart0.xyz

[J03] 字符串解析为日期
来源：http://mir.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bbi.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ozm.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://fpp.tarul.cn

TS:   new Date("2024-01-02")
来源：http://prn.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://jmw.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kyx.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://jhq.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://htn.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://zqz.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jog.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cyp.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qpw.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mpb.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ngr.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zho.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kfg.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bnz.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://qjw.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://vbt.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://epx.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://knb.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://knt.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://tcn.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hcu.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://sae.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://cbl.316326.xyz

[J06] 计算两时间之差
来源：http://zfp.hesvh.cn


<!-- 参考信息 -->