代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://rrg.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://ouk.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://edf.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://qtu.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://jtr.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://ahe.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vub.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://yby.shanyushiyangtech.top

[G10] 访问控制
来源：http://xas.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://ygz.xuetiantiany.cn

PHP:  public / protected / private
来源：http://mad.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://yyk.daria6918.cn

TS:   public / protected / private
来源：http://vss.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://dvw.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dah.fengsongda.top

Ruby: public / protected / private
来源：http://uit.jianghu66.top

C#:   public / protected / private / internal
来源：http://ylr.yfazqb.com

[G11] getter / setter
来源：http://qfl.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://knx.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eha.fehbvm.com

JS:   get name() { return this._name; }
来源：http://xzk.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://fej.ctjpmb.com

Java: public String getName() { return name; }
来源：http://vqm.fanxiaobao.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://atn.0kj1m.cn

Ruby: attr_accessor :name
来源：http://oov.vehdjk.com

C#:   public string Name { get; set; }
来源：http://khf.aizwys.cn

[G12] 对象转字符串
来源：http://ryy.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://ikw.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://tmq.guannengcc.top

JS:   toString() { return this.name; }
来源：http://wzr.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://ipy.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://ueq.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://egq.aizwys.cn

Ruby: def to_s; @name; end
来源：http://cmt.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://xdq.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://qop.jqgfzy.top

Py:   isinstance(u, User)
来源：http://vav.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://zew.ehwqpu.com

JS:   u instanceof User
来源：http://vfb.aibaodan.cn

TS:   u instanceof User
来源：http://fkw.sxryk.cn

Java: u instanceof User
来源：http://tgg.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xgn.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://vfa.ybcxt.top

C#:   u is User
来源：http://jmz.haohaochexian.top

[G14] 数据类 / record
来源：http://uiv.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qbf.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://jrg.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://tid.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://ruc.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://rrv.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://oni.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fpv.yj20258.top

C#:   record User(string Name, int Age);
来源：http://xjg.yuxming.cn

[G15] 枚举
来源：http://hph.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xns.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ajr.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vfj.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zzz.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://hiy.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dum.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://fgs.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gyr.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://xjo.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rnk.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://ntm.yuxming.cn

JS:   Object.entries(obj)
来源：http://ikv.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://xjk.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://axo.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ghn.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://qzn.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://oka.yfazqb.com

================================================================================
来源：http://cxt.uphjek.com

H. 异常与错误处理
来源：http://ner.feifeiyinyue.top

================================================================================
来源：http://xaq.jqgufenzy.top

[H01] try / catch 基础
来源：http://mjo.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hnz.fehbvm.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ygi.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vzb.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vsv.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rng.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://apf.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tqi.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jus.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://pqj.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ker.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cki.guowangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lym.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://crw.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pgo.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kpv.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qdo.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qik.aizwys.cn

[H03] 主动抛出异常
来源：http://scq.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://iua.fehbvm.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yvp.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://wpj.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://brw.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hqu.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uky.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mda.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jek.havefunace.top

[H04] 自定义异常类型
来源：http://qwd.yj202588.top

Py:   class MyError(Exception): pass
来源：http://irv.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://znr.cheryme.top

JS:   class MyError extends Error {}
来源：http://xsd.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://jlb.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://fke.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eng.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://ekx.ybcxt.top

C#:   class MyException : Exception {}
来源：http://fze.zhoulong.xyz

[H05] 捕获特定类型
来源：http://cvm.hcnkem.com

Py:   except ValueError as e:
来源：http://oxd.ppjwa.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rrw.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://txa.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://gel.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://fsn.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://njz.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://yfp.zhaomingkeji.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://edz.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://aop.ybcxt.top

Py:   value = d.get("k") or default
来源：http://cel.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://act.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://kjc.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://clj.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uuy.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yit.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://dgk.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://obl.jinqigufen.top

[H07] 断言
来源：http://tqn.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://pmq.cashguo.top

PHP:  assert($x > 0);
来源：http://ykg.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://xll.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://lti.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://nhg.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eof.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ist.c1oappe.top

C#:   Debug.Assert(x > 0);
来源：http://qhf.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://gxs.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://shy.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jja.ybcxt.top

JS:   e.message;  e.stack
来源：http://qlh.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://slw.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gzj.sweek.top

Go:   err.Error()
来源：http://hvp.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://ouj.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://auf.daxiang520.top

[H09] 带错误码的异常
来源：http://ayq.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wco.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nhx.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wje.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://crh.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ryb.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://woq.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lgk.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yfj.aibaodan.cn

[H10] 资源自动释放
来源：http://gim.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://twk.zhixingplan.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rbt.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qiy.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cuz.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cib.fktsv.cn

Go:   defer f.Close()
来源：http://uku.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kbo.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xpv.feifeiyinyue.top

================================================================================
来源：http://jyb.hnqzz.top

I. 正则表达式
来源：http://puu.yj20258888.top

================================================================================
来源：http://rlt.yuxming.cn

[I01] 判断是否匹配
来源：http://whd.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vaj.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kgy.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://ise.iojbl.cn

TS:   /\d+/.test(s)
来源：http://lrk.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wua.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xwr.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://oic.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://esy.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://pra.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://oxq.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eai.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewy.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://trt.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jsb.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pwh.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://xnx.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://neh.xziqi.cn

[I03] 提取捕获分组
来源：http://akd.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lcm.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://udq.xziqi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hlh.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pjf.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://khw.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aje.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bql.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://daj.wangdashe.top

[I04] 正则替换
来源：http://haj.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iqi.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oll.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://igw.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://mss.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://nyp.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://npv.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kyb.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ufy.vqdsnc.cn

[I05] 按正则拆分
来源：http://hcy.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pyb.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pir.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://atv.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://fzj.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://vse.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xkh.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://rtp.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hka.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kaj.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vnj.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://etv.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zth.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwv.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hvi.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pff.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vkw.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xff.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://bhd.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gzu.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bgs.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mhg.dianchejie.cn

TS:   /error/gim
来源：http://xhl.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bfe.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqg.uphjek.com

Ruby: s.scan(/error/i)
来源：http://fqy.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fcq.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ygk.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cuh.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ijl.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fpm.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbb.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bku.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mha.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rkg.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lay.zhiwuduotai.top

================================================================================
来源：http://gdi.zhixingplan.top

J. 日期与时间
来源：http://qcf.vqdsnc.cn

================================================================================
来源：http://enu.birdmap.top

[J01] 获取当前时间
来源：http://flm.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://edq.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lnf.jianghu66.top

JS:   new Date();  Date.now()
来源：http://pul.yongpay.top

TS:   new Date();  Date.now()
来源：http://kmf.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://pnf.jyoumei.cn

Go:   time.Now()
来源：http://eou.chenzaomai.com

Ruby: Time.now
来源：http://vep.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nfe.feifeiyinyue.top

[J02] 格式化输出
来源：http://mko.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ept.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ren.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rcl.jiagoushi.top

TS:   d.toISOString()
来源：http://alz.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qaj.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cye.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xkv.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gmq.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://ggi.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bkz.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://doo.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://tky.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://iri.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://fqx.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://orx.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://ohc.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okg.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://fox.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bvy.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ovd.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zts.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fov.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mqc.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bwh.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qsr.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yfm.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://mjk.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://kkt.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yzg.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdw.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpt.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://jdq.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kgb.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://oox.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://cxo.vehdjk.com

[J06] 计算两时间之差
来源：http://nhu.pycfn.com

Py:   (end - start).total_seconds()
来源：http://grw.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://tli.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vlh.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wua.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://sjy.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://ose.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://lzl.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://wkn.aizwys.cn

[J07] 比较两个日期
来源：http://iku.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://ows.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gdp.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://tex.fzhhl.top


<!-- 参考信息 -->