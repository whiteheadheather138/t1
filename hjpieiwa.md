代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://pnt.jlsjyb.cn

Ruby: def self.f; end
来源：http://ofn.chenlongwang.top

C#:   public static void F() {}
来源：http://xcx.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://jvs.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://htj.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ylh.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vqj.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://isc.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://orq.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://prr.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dtd.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://xqp.hammf.cn

[G10] 访问控制
来源：http://urm.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://wqw.vehdjk.com

PHP:  public / protected / private
来源：http://ukq.xuanzx.com

JS:   #private 字段；其余公开
来源：http://mfk.shanyushiyangtech.top

TS:   public / protected / private
来源：http://rbh.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://aka.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvm.guowangkeji.top

Ruby: public / protected / private
来源：http://xvt.yuxming.cn

C#:   public / protected / private / internal
来源：http://cjs.fzhhl.top

[G11] getter / setter
来源：http://bgv.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://tys.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ulu.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://yku.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://tlj.gogol.net.cn

Java: public String getName() { return name; }
来源：http://szx.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://znm.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://vnx.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://ngx.jiagoushi.top

[G12] 对象转字符串
来源：http://zcp.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://mhw.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qhd.316326.xyz

JS:   toString() { return this.name; }
来源：http://oqa.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://naf.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://dpg.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://uhp.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://hia.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://mrl.zdqjudy.top

[G13] 判断对象类型
来源：http://ujt.xinyue.icu

Py:   isinstance(u, User)
来源：http://hwy.xinyue.icu

PHP:  $u instanceof User
来源：http://rnk.fanxiaobao.xyz

JS:   u instanceof User
来源：http://meb.quarkkingdee.top

TS:   u instanceof User
来源：http://lbz.chenjidiqi.icu

Java: u instanceof User
来源：http://rgs.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bkq.hnqzz.top

Ruby: u.is_a?(User)
来源：http://ajv.dianchejie.cn

C#:   u is User
来源：http://kah.haohaochexian.top

[G14] 数据类 / record
来源：http://mkw.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://brc.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://ank.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vaf.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://fmr.yj20258888.top

Java: record User(String name, int age) {}
来源：http://xah.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://ell.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://diw.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://qvp.xylfe.cn

[G15] 枚举
来源：http://yoc.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ern.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://yav.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rhw.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rkw.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://tjp.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdi.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://ygl.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ovn.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://eqp.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ycx.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://qmm.zdbjq.cn

JS:   Object.entries(obj)
来源：http://utv.snrcjt.cn

TS:   Object.entries(obj)
来源：http://jdn.guowangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwo.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vnb.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://nnm.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://cwo.jinqigufen.top

================================================================================
来源：http://eia.ydjk.org.cn

H. 异常与错误处理
来源：http://aoh.chenlongwang.top

================================================================================
来源：http://oxu.daxiang520.top

[H01] try / catch 基础
来源：http://zxx.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mwc.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nle.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://agp.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://njd.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qsg.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hfg.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ggi.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wsh.cashguo.top

[H02] finally / ensure 收尾
来源：http://bsj.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tjv.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eqd.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zbj.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://sfe.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://ysq.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lss.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dwb.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://etz.9152youxi.cn

[H03] 主动抛出异常
来源：http://ogp.sweek.top

Py:   raise ValueError("错误信息")
来源：http://cmt.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ske.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://fzr.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://tle.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zgo.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rsg.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uqe.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://xoj.hnqzz.top

[H04] 自定义异常类型
来源：http://ojv.meibo888.top

Py:   class MyError(Exception): pass
来源：http://btb.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://ruy.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://tgy.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://oss.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://pre.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rru.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://swr.daxiang520.top

C#:   class MyException : Exception {}
来源：http://owh.havefunace.top

[H05] 捕获特定类型
来源：http://txx.jyoumei.cn

Py:   except ValueError as e:
来源：http://sku.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oks.uphjek.com

JS:   if (e instanceof TypeError) {}
来源：http://rob.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://weg.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://qcd.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hjv.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://wnb.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xzx.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://cdb.tian-w.cn

Py:   value = d.get("k") or default
来源：http://vrz.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://syw.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://khh.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://fiv.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dlw.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fol.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://oev.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://yop.yuxming.cn

[H07] 断言
来源：http://ldz.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://dnr.xylfe.cn

PHP:  assert($x > 0);
来源：http://ziy.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://qff.xylfe.cn

TS:   console.assert(x > 0);
来源：http://viy.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://jml.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nts.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://ccj.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://rbj.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://ddp.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://yjk.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lsk.fengsongda.top

JS:   e.message;  e.stack
来源：http://rto.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lqk.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lee.epnwcf.com

Go:   err.Error()
来源：http://xum.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://zyg.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://ipj.birdmap.top

[H09] 带错误码的异常
来源：http://szg.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hhb.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xdr.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lya.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kxg.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mgm.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rok.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vkd.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jle.hesvh.cn

[H10] 资源自动释放
来源：http://eae.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://znx.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ttr.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ukt.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qvu.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lhm.uphjek.com

Go:   defer f.Close()
来源：http://evo.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hxs.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qrh.zdqjudy.top

================================================================================
来源：http://jml.yj20258888.top

I. 正则表达式
来源：http://nxl.fzhhl.top

================================================================================
来源：http://vjz.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://two.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pvo.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://fjv.316326.xyz

JS:   /\d+/.test(s)
来源：http://nxi.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://waz.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xyd.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ogx.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://qqz.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gna.gotoacloud.top

[I02] 提取所有匹配
来源：http://wea.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://iry.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffs.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nbu.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://vok.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xgr.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://man.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://iwc.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gig.9152youxi.cn

[I03] 提取捕获分组
来源：http://wfh.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://adv.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ixd.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wyk.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgu.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wuh.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gmm.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eog.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dkb.sxryk.cn

[I04] 正则替换
来源：http://rgo.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hiu.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uor.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://tsh.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://emo.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://cwl.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wfa.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jmy.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mdo.shzxlz.cn

[I05] 按正则拆分
来源：http://nte.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://snz.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://osz.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://vip.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://miq.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://fvt.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://byr.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ipu.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uwr.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qkz.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pbz.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hlg.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://klo.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mes.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oej.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mss.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vmg.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://otd.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://ixq.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lbf.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://way.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qim.bbcook.cn

TS:   /error/gim
来源：http://yfh.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxx.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://klq.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://ovd.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ewy.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://kzo.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ypi.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pht.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uqy.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqw.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vvc.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pts.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cjm.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvr.shzxlz.cn

================================================================================
来源：http://mvg.guowangkeji.top

J. 日期与时间
来源：http://wzk.birdmap.top

================================================================================
来源：http://idg.nanxuanxn.top

[J01] 获取当前时间
来源：http://mfu.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ogg.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xte.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://vne.sysykeji.top

TS:   new Date();  Date.now()
来源：http://xne.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fci.zhaomingkeji.xyz

Go:   time.Now()
来源：http://xod.aibaodan.cn

Ruby: Time.now
来源：http://ilw.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gfz.chenlongwang.top

[J02] 格式化输出
来源：http://fcz.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://egx.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mqj.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://irk.cqqwz.cn

TS:   d.toISOString()
来源：http://oom.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xld.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://erz.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mgw.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pql.xinyue.icu

[J03] 字符串解析为日期
来源：http://ydo.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xjw.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yyj.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://wzu.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://wha.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cme.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rxh.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://vcg.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bij.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://unn.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jji.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fnl.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://euk.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bge.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xvx.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tos.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qlq.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vgl.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://bqz.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://rka.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://icd.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qkz.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhk.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://mkn.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ljk.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://pyd.svipenyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fva.daxiang520.top

[J06] 计算两时间之差
来源：http://zbg.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://lnn.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://spg.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cqm.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kia.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://naq.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://wsg.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://cjs.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://nfz.bbcook.cn


<!-- 参考信息 -->