代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://vgr.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ajf.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zmx.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://pdt.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://dfl.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://upx.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://avu.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://jth.xziqi.cn

[G10] 访问控制
来源：http://bzw.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://fpa.cqqwz.cn

PHP:  public / protected / private
来源：http://wnd.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://jfd.redwolf501.top

TS:   public / protected / private
来源：http://cwa.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://idx.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://vhb.jiagoushi.top

Ruby: public / protected / private
来源：http://yby.ppjwa.cn

C#:   public / protected / private / internal
来源：http://voo.shzxlz.cn

[G11] getter / setter
来源：http://tkn.shuidangran.top

Py:   @property 与 @x.setter
来源：http://ymv.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gnb.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://bsh.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://jxf.dashuyun.cn

Java: public String getName() { return name; }
来源：http://djl.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ecg.yj20258888.top

Ruby: attr_accessor :name
来源：http://ykn.hammf.cn

C#:   public string Name { get; set; }
来源：http://ubp.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://hhv.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://eoc.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eez.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://seg.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://kmo.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://vbc.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://cpd.bbcook.cn

Ruby: def to_s; @name; end
来源：http://gsy.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://txl.quarkkingdee.top

[G13] 判断对象类型
来源：http://toy.zhengqikj.top

Py:   isinstance(u, User)
来源：http://kzs.dianchejie.cn

PHP:  $u instanceof User
来源：http://ulw.svipenyu.cn

JS:   u instanceof User
来源：http://dkr.quarkkingdee.top

TS:   u instanceof User
来源：http://sza.gzhubu.top

Java: u instanceof User
来源：http://czx.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tag.bjfxy.top

Ruby: u.is_a?(User)
来源：http://wpv.chenlongwang.top

C#:   u is User
来源：http://ehc.fehbvm.com

[G14] 数据类 / record
来源：http://rpr.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jnx.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://ebj.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wmo.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://bwk.hcnkem.com

Java: record User(String name, int age) {}
来源：http://hth.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://uhq.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nhy.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://frn.tianlin.xyz

[G15] 枚举
来源：http://lwj.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dfr.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://jpw.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hhn.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wdx.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://sri.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yzu.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://bpe.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wjp.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://esa.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qya.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://gew.vehdjk.com

JS:   Object.entries(obj)
来源：http://oro.tianlin.xyz

TS:   Object.entries(obj)
来源：http://sbe.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://chp.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ofj.ivvv.top

Ruby: obj.instance_variables
来源：http://yvh.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://pzw.hysaishi.cn

================================================================================
来源：http://fnf.hammf.cn

H. 异常与错误处理
来源：http://zcf.jinqigufen.top

================================================================================
来源：http://gyl.nanxinkj.top

[H01] try / catch 基础
来源：http://ijs.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://auk.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mzb.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyu.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ldt.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kjc.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bcj.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xpb.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oud.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://hps.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://xnj.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rnz.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kbz.hysaishi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hon.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jjm.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lfh.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jym.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://zqk.tanke756.top

[H03] 主动抛出异常
来源：http://aam.chenzaomai.com

Py:   raise ValueError("错误信息")
来源：http://dnk.yueranfly.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vja.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://vfk.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://kij.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://oyy.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ezz.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ots.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mcj.yj20258.top

[H04] 自定义异常类型
来源：http://jmb.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://gmu.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jae.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://urs.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://apy.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://pnk.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eow.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://ush.zycfv.cn

C#:   class MyException : Exception {}
来源：http://ift.hnxiangtu.top

[H05] 捕获特定类型
来源：http://sdv.yongpay.top

Py:   except ValueError as e:
来源：http://gag.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://omx.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://ifd.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://izi.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://mas.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://znc.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://asi.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uab.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://fmq.guannengcc.top

Py:   value = d.get("k") or default
来源：http://jjt.vehdjk.com

PHP:  $v = $d["k"] ?? null;
来源：http://qhg.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://brt.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://azs.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ogd.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cin.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://yrw.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://rli.jinghuilouyu.cn

[H07] 断言
来源：http://vqn.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://obr.sxryk.cn

PHP:  assert($x > 0);
来源：http://pwj.gzhubu.top

JS:   console.assert(x > 0);
来源：http://qjb.aizwys.cn

TS:   console.assert(x > 0);
来源：http://rzb.guannengcc.top

Java: assert x > 0 : "必须为正";
来源：http://crw.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://npl.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://xeh.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://ypl.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://ymb.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://pup.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kaf.gogol.net.cn

JS:   e.message;  e.stack
来源：http://yjs.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ofx.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://nwh.hysaishi.cn

Go:   err.Error()
来源：http://dmv.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://dat.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://tnk.yonumen.top

[H09] 带错误码的异常
来源：http://dfp.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oak.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://uuf.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kec.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ezg.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cmr.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gcu.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tfa.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tim.svipenyu.cn

[H10] 资源自动释放
来源：http://xrn.0kj1m.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://taz.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tpw.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lvy.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qvw.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mra.andypj.xyz

Go:   defer f.Close()
来源：http://awo.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wgw.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kwe.iojbl.cn

================================================================================
来源：http://ees.guowangkeji.top

I. 正则表达式
来源：http://flo.yanxiufei.cn

================================================================================
来源：http://tzv.snrcjt.cn

[I01] 判断是否匹配
来源：http://tfu.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://agp.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nbx.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://lre.52xcode.cn

TS:   /\d+/.test(s)
来源：http://bhg.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wjc.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://foq.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://kqp.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mic.svipenyu.cn

[I02] 提取所有匹配
来源：http://dzf.jqgufenzy.top

Py:   re.findall(r"\d+", s)
来源：http://dgt.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kcl.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://spk.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://lyg.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oxs.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://seu.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://vtg.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zxo.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://afn.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rxn.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gah.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xhy.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gay.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://thr.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndd.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xxn.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iec.yanxiufei.cn

[I04] 正则替换
来源：http://qyy.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cht.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oqi.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://egk.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://txk.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://dzn.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mdz.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qqc.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vqf.yj202588.top

[I05] 按正则拆分
来源：http://wew.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pgk.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjv.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://uyl.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://owg.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://sfk.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oar.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gjr.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zsx.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://plt.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://smz.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tro.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cms.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://maj.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lze.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vlt.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kmz.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ewp.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://ksy.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ria.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mzd.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rrp.redwolf501.top

TS:   /error/gim
来源：http://uok.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hie.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xqs.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://aab.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fxp.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://vwy.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://upg.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfl.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://imt.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://odj.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yeb.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fba.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dqb.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zsd.jinghuilouyu.cn

================================================================================
来源：http://igs.fehbvm.com

J. 日期与时间
来源：http://egm.aibaodan.cn

================================================================================
来源：http://yhi.0kj1m.cn

[J01] 获取当前时间
来源：http://tkw.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://phd.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hcj.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://xua.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://vci.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://moy.hammf.cn

Go:   time.Now()
来源：http://tay.ivvv.top

Ruby: Time.now
来源：http://qso.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eso.yuxming.cn

[J02] 格式化输出
来源：http://xag.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqc.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cnb.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wdk.zhiwuduotai.top

TS:   d.toISOString()
来源：http://dnf.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://req.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yyj.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zve.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://slu.meibo888.top

[J03] 字符串解析为日期
来源：http://spj.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zqy.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://obk.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://xxz.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://avw.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://tec.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bps.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://wde.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tgm.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://fpo.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cyu.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://isx.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ksn.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wpj.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://enx.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bwq.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://opv.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mdp.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://kbh.pycfn.com

Py:   now + timedelta(days=7)
来源：http://iej.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zpn.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://szb.yfazqb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yeu.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://ruz.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brb.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://qii.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://svv.hysaishi.cn

[J06] 计算两时间之差
来源：http://zga.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://cmc.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://bbu.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jwv.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mlg.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://hph.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://pig.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://eya.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://peh.zhongyouzk.top

[J07] 比较两个日期
来源：http://viz.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://rql.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wvd.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gib.andypj.xyz


<!-- 参考信息 -->