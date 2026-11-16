代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://tyg.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://vun.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://nxf.52xcode.cn

[G09] 接口 / 抽象类
来源：http://wmg.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://bwa.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://men.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://qck.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://rgp.yj202588.top

Java: interface Shape { double area(); }
来源：http://ylr.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://ioc.aibaodan.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wkb.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://qrw.chenlongwang.top

[G10] 访问控制
来源：http://fju.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://jvk.zhijiandao.cn

PHP:  public / protected / private
来源：http://znk.52xcode.cn

JS:   #private 字段；其余公开
来源：http://pym.haohaochexian.top

TS:   public / protected / private
来源：http://pea.meibo888.top

Java: public / protected / private / 默认包级
来源：http://pzd.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://akl.vehdjk.com

Ruby: public / protected / private
来源：http://qmt.tian-w.cn

C#:   public / protected / private / internal
来源：http://jdg.epnwcf.com

[G11] getter / setter
来源：http://xas.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://svg.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uat.fzhhl.top

JS:   get name() { return this._name; }
来源：http://vmr.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://msf.tarul.cn

Java: public String getName() { return name; }
来源：http://ikk.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jaz.epnwcf.com

Ruby: attr_accessor :name
来源：http://kdb.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://qtq.jinqigufen.top

[G12] 对象转字符串
来源：http://uiu.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://awx.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://bsx.yvedp.cn

JS:   toString() { return this.name; }
来源：http://nlx.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://cwc.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://vjz.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://wsm.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://ybh.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://uqc.dianchejie.cn

[G13] 判断对象类型
来源：http://vzp.hnqzz.top

Py:   isinstance(u, User)
来源：http://bjq.meibo888.top

PHP:  $u instanceof User
来源：http://jxh.ybcxt.top

JS:   u instanceof User
来源：http://nvv.hysaishi.cn

TS:   u instanceof User
来源：http://jvm.yanxiufei.cn

Java: u instanceof User
来源：http://ord.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nrs.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://kkk.zhijiandao.cn

C#:   u is User
来源：http://ifh.gogol.net.cn

[G14] 数据类 / record
来源：http://zrg.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ngb.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://zrx.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://zpq.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://ilp.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://enw.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://sjs.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qgg.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://djt.yj202588.top

[G15] 枚举
来源：http://jzr.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ebr.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://qri.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wgw.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ekd.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://qxj.ydjk.org.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zba.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://ohq.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijb.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://pzd.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jrk.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://kfs.svipenyu.cn

JS:   Object.entries(obj)
来源：http://cdy.yj20258888.top

TS:   Object.entries(obj)
来源：http://bmy.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ivy.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lxu.zycfv.cn

Ruby: obj.instance_variables
来源：http://xee.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://jmt.birdmap.top

================================================================================
来源：http://cfo.gaohongyu789.top

H. 异常与错误处理
来源：http://ccx.yonumen.top

================================================================================
来源：http://eng.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://mwq.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jps.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ewe.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozo.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zoj.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jfe.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sol.fzhhl.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tam.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dzj.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://cni.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://scf.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://vhh.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vus.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zpt.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://ffi.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hae.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nho.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vjm.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://wbg.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://div.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jnp.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://jjd.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://rkb.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hva.wangshuangyany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://esi.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ina.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://gif.316326.xyz

[H04] 自定义异常类型
来源：http://lve.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://lhd.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://vwz.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://pyd.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://dvx.316326.xyz

Java: class MyException extends RuntimeException {}
来源：http://bdl.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://muw.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://lei.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://gah.snrcjt.cn

[H05] 捕获特定类型
来源：http://agh.yangfankeji.com

Py:   except ValueError as e:
来源：http://qkb.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rcw.gzhubu.top

JS:   if (e instanceof TypeError) {}
来源：http://mmb.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://kbb.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nhz.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jxs.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://sft.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xud.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://bme.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://dvw.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://buv.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fcd.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://otw.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ibk.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xtz.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://zhn.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://apx.hnxiangtu.top

[H07] 断言
来源：http://ege.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://bhq.nwbrower.top

PHP:  assert($x > 0);
来源：http://oad.hcnkem.com

JS:   console.assert(x > 0);
来源：http://mmh.uphjek.com

TS:   console.assert(x > 0);
来源：http://haq.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://dnz.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ify.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://lgg.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://hzn.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://frt.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://yza.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xie.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://ejq.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://qfk.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nuo.haohaochexian.top

Go:   err.Error()
来源：http://zkr.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://hpu.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://wwv.xylfe.cn

[H09] 带错误码的异常
来源：http://nhg.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gel.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zsv.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zbx.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wrc.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ayb.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bir.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ana.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://chm.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://dpr.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qlv.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yrg.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bte.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iig.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nsg.redwolf501.top

Go:   defer f.Close()
来源：http://hwp.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pga.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://coc.yfazqb.com

================================================================================
来源：http://qyx.bbcook.cn

I. 正则表达式
来源：http://wss.fanxiaobao.xyz

================================================================================
来源：http://plp.guannengcc.top

[I01] 判断是否匹配
来源：http://tea.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xxk.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://uvp.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://gez.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://zog.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://omm.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vzk.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://uen.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dua.yongpay.top

[I02] 提取所有匹配
来源：http://umw.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://cwa.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mpr.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hyo.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://nhn.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xbv.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dzg.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://tqv.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cvc.gotoacloud.top

[I03] 提取捕获分组
来源：http://tuv.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rpx.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zaq.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lyk.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://csd.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://svq.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zcv.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://msq.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rfc.tanke756.top

[I04] 正则替换
来源：http://igc.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uxu.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzr.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://wlt.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://uby.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://fxn.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nxi.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bta.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qfx.hywenlv.cn

[I05] 按正则拆分
来源：http://ubw.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vxy.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fdr.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://mpq.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://orm.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://opb.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rxj.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://iiy.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mtb.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://slp.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ovu.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nwb.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goj.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mez.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bgn.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uua.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wvu.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eqk.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://yrb.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://udn.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgl.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bso.tian-w.cn

TS:   /error/gim
来源：http://jbz.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oeq.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://alr.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://stk.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tee.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://bsk.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ryj.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lfl.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xou.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://orq.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tob.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lud.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qim.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://upp.yj20258888.top

================================================================================
来源：http://itz.shuidangran.top

J. 日期与时间
来源：http://aer.mhx1999.top

================================================================================
来源：http://web.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://gmy.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://vuy.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ryv.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://fak.guannengcc.top

TS:   new Date();  Date.now()
来源：http://ino.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ban.jianghu66.top

Go:   time.Now()
来源：http://imc.tianlin.xyz

Ruby: Time.now
来源：http://mak.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bsx.9152youxi.cn

[J02] 格式化输出
来源：http://yks.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzk.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ehg.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qyq.jinqigfzy.top

TS:   d.toISOString()
来源：http://pcc.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jot.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://twl.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lck.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://stx.snrcjt.cn

[J03] 字符串解析为日期
来源：http://pre.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sdr.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypc.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://dpk.tanke756.top

TS:   new Date("2024-01-02")
来源：http://hbc.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://emh.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozv.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://kat.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://poe.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://iaf.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vmd.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hhw.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://npw.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ahd.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vbh.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lgz.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zhr.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ala.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://vml.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://qkr.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nuh.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://efs.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gap.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://mpz.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fpx.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://beq.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://hew.uphjek.com

[J06] 计算两时间之差
来源：http://dyh.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://lbi.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://tjz.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uug.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://int.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://blm.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://rni.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://xgb.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://mjb.jinyuanbaomall.cn


<!-- 参考信息 -->