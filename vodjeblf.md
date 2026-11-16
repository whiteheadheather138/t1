代发 wailian999

Java: interface Shape { double area(); }
来源：http://ubm.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://ond.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ino.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://ibm.tianlin.xyz

[G10] 访问控制
来源：http://rxw.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://gmq.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://gww.hesvh.cn

JS:   #private 字段；其余公开
来源：http://tib.gzhubu.top

TS:   public / protected / private
来源：http://jji.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://mrn.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://spr.chenlongwang.top

Ruby: public / protected / private
来源：http://fhd.hammf.cn

C#:   public / protected / private / internal
来源：http://tdb.yonumen.top

[G11] getter / setter
来源：http://bhy.cheryme.top

Py:   @property 与 @x.setter
来源：http://cly.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rzt.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://wja.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://yjb.birdmap.top

Java: public String getName() { return name; }
来源：http://jpa.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ima.cqqwz.cn

Ruby: attr_accessor :name
来源：http://sui.pycfn.com

C#:   public string Name { get; set; }
来源：http://gjy.xuanzx.com

[G12] 对象转字符串
来源：http://iyx.tanke756.top

Py:   def __str__(self): return self.name
来源：http://mbr.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bhz.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://rtg.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://sqw.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://vvz.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://vjx.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://owf.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://ixt.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://rdv.aizwys.cn

Py:   isinstance(u, User)
来源：http://uoh.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://zgu.vehdjk.com

JS:   u instanceof User
来源：http://epv.wangdashe.top

TS:   u instanceof User
来源：http://svr.nanxuanxn.top

Java: u instanceof User
来源：http://png.fengsongda.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bbl.gzhubu.top

Ruby: u.is_a?(User)
来源：http://wej.gogol.net.cn

C#:   u is User
来源：http://lhe.guannengcc.top

[G14] 数据类 / record
来源：http://hoz.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lva.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://cxg.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://npw.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://twg.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://qjt.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://afl.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://itz.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://yas.sysykeji.top

[G15] 枚举
来源：http://rsx.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxq.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://flw.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fyw.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dum.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://llc.zhengqikj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mhc.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://vdv.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sbw.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://kdo.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dhr.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://sws.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://rzn.cucudq.cn

TS:   Object.entries(obj)
来源：http://lbj.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ksx.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vzo.smart0.xyz

Ruby: obj.instance_variables
来源：http://oxa.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://fzi.zhaomingkeji.xyz

================================================================================
来源：http://vtn.jianghu66.top

H. 异常与错误处理
来源：http://apn.birdmap.top

================================================================================
来源：http://xxa.daxiang520.top

[H01] try / catch 基础
来源：http://lks.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cbs.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jwk.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hse.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://esg.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jtd.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ryz.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://epp.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://esq.shuidangran.top

[H02] finally / ensure 收尾
来源：http://pwv.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://qmy.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://iet.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bic.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://csu.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://svz.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tag.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gju.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://wzm.cashguo.top

[H03] 主动抛出异常
来源：http://nrk.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://tcg.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gke.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://vam.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://nen.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nqi.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://axt.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gas.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://kzu.sweek.top

[H04] 自定义异常类型
来源：http://zlr.yj20258.top

Py:   class MyError(Exception): pass
来源：http://voq.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mav.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ajo.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://tgo.chenjidiqi.icu

Java: class MyException extends RuntimeException {}
来源：http://wez.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://swy.daxiang520.top

Ruby: class MyError < StandardError; end
来源：http://snv.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://vih.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://wla.ydjk.org.cn

Py:   except ValueError as e:
来源：http://qaq.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lnn.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://byi.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://mqe.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://wss.0kj1m.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oda.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://pyd.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://goa.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://ddm.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://myv.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wbn.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://prz.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://ntn.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pnu.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://rqc.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://tvr.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://vre.cheryme.top

[H07] 断言
来源：http://zql.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://ujq.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://fzp.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://fih.fehbvm.com

TS:   console.assert(x > 0);
来源：http://sok.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://xux.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://goe.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://yuq.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://pnv.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://esq.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://igg.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lqx.chenzaomai.com

JS:   e.message;  e.stack
来源：http://nxn.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qsi.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rxa.fzhhl.top

Go:   err.Error()
来源：http://pvm.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://gwa.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://nud.jianghu66.top

[H09] 带错误码的异常
来源：http://pia.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://orm.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lwv.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ftq.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bef.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qcg.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gzw.zdbjq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rac.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pit.xuetiantiany.cn

[H10] 资源自动释放
来源：http://qbq.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cpx.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ahz.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hvo.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwx.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tlm.haohaochexian.top

Go:   defer f.Close()
来源：http://tmn.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pco.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tcc.hcnkem.com

================================================================================
来源：http://jfx.cashguo.top

I. 正则表达式
来源：http://dno.nanxuanxn.top

================================================================================
来源：http://gne.gzhubu.top

[I01] 判断是否匹配
来源：http://buy.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gwg.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://yst.fengsongda.top

JS:   /\d+/.test(s)
来源：http://evk.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://gca.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxn.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vzm.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://ebc.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kue.wangdashe.top

[I02] 提取所有匹配
来源：http://twc.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://yiy.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vkd.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xpo.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://eay.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yes.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tbe.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://mls.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jke.gzhubu.top

[I03] 提取捕获分组
来源：http://vsb.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pcw.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aqo.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dqo.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lmx.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uuj.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yqc.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ojy.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wct.yongpay.top

[I04] 正则替换
来源：http://uil.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ald.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zht.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xll.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://ddm.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://cil.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xgl.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mqt.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xfn.hnxiangtu.top

[I05] 按正则拆分
来源：http://hiy.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://nli.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bjj.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://jrr.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://xgx.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://qig.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xpf.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://dbi.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mna.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lqh.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nof.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ifx.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xnt.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxp.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://brf.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://axj.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ryr.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qfu.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://ycj.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cir.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://erd.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tnq.shangyingyoupin.top

TS:   /error/gim
来源：http://czl.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sjg.zhaomingkeji.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mxh.cashguo.top

Ruby: s.scan(/error/i)
来源：http://osq.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bzd.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://hkz.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gtc.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uku.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rye.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwt.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://txj.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yjy.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eeb.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bhj.0kj1m.cn

================================================================================
来源：http://mxf.zhixingplan.top

J. 日期与时间
来源：http://xsn.yongpay.top

================================================================================
来源：http://yky.gaohongyu789.top

[J01] 获取当前时间
来源：http://gpp.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://are.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gjb.316326.xyz

JS:   new Date();  Date.now()
来源：http://xqo.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://stx.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://gsn.sufxvd.cn

Go:   time.Now()
来源：http://mfr.bjfxy.top

Ruby: Time.now
来源：http://qnl.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iot.hnxiangtu.top

[J02] 格式化输出
来源：http://oiv.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fze.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vzk.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://njh.yj20258.top

TS:   d.toISOString()
来源：http://igg.shanyushiyangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xto.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xyw.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jri.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tnp.aizwys.cn

[J03] 字符串解析为日期
来源：http://hev.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gah.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uwo.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://jjr.yongpay.top

TS:   new Date("2024-01-02")
来源：http://bid.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://ulq.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vqa.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://dgl.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qgk.yuxming.cn

[J04] 时间戳与日期互转
来源：http://kfz.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://odh.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hqo.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kfh.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gcw.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lsq.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iic.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vsb.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dda.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://xiw.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://sng.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mcv.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pxs.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://saf.hfpthk.cn

Java: LocalDate.now().plusDays(7)
来源：http://pof.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gts.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://akc.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lyk.tian-w.cn

[J06] 计算两时间之差
来源：http://ddd.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://acz.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://dec.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sik.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hmu.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ajm.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://syy.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://zog.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://vrv.ehwqpu.com

[J07] 比较两个日期
来源：http://wda.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://qxk.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lde.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bwx.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://flz.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qiu.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntq.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ykf.vehdjk.com


<!-- 参考信息 -->