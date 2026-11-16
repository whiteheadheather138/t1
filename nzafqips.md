代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://lvv.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://ovz.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://axu.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://edf.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://slb.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://qlh.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kvf.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://yvh.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://jqq.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://igy.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ory.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://ytr.ctjpmb.com

[G10] 访问控制
来源：http://hma.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://aks.yj20258888.top

PHP:  public / protected / private
来源：http://hwk.tian-w.cn

JS:   #private 字段；其余公开
来源：http://pdw.yuanzhike.top

TS:   public / protected / private
来源：http://qkk.pycfn.com

Java: public / protected / private / 默认包级
来源：http://ivh.pengpengdd.cyou

Go:   首字母大写可导出，小写仅包内可见
来源：http://jfe.chenjidiqi.icu

Ruby: public / protected / private
来源：http://icu.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://www.c1oappe.top

[G11] getter / setter
来源：http://vxw.zycfv.cn

Py:   @property 与 @x.setter
来源：http://zec.guowangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lej.daria6918.cn

JS:   get name() { return this._name; }
来源：http://yak.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://zuq.xinyue.icu

Java: public String getName() { return name; }
来源：http://pmj.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xhl.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://grd.meibo888.top

C#:   public string Name { get; set; }
来源：http://slz.yuxming.cn

[G12] 对象转字符串
来源：http://gmz.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://dsd.ehwqpu.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://syi.gzhubu.top

JS:   toString() { return this.name; }
来源：http://iqz.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://lea.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://ipm.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://rvo.yueranfly.top

Ruby: def to_s; @name; end
来源：http://voq.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://ico.shangyingyoupin.top

[G13] 判断对象类型
来源：http://bkh.hcnkem.com

Py:   isinstance(u, User)
来源：http://zay.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://wlb.tanke756.top

JS:   u instanceof User
来源：http://nyz.fktsv.cn

TS:   u instanceof User
来源：http://zlg.nwbrower.top

Java: u instanceof User
来源：http://dlo.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nju.zycfv.cn

Ruby: u.is_a?(User)
来源：http://sel.hongshengwenyu.top

C#:   u is User
来源：http://rff.jiagoushi.top

[G14] 数据类 / record
来源：http://wvd.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uum.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://orq.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://jok.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://njv.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://jig.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://jfk.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gyn.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://bpn.zhaomingkeji.xyz

[G15] 枚举
来源：http://gxu.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://enp.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kdm.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oqy.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lev.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://hia.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uuw.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://ses.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://trf.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://xao.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iqg.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://mli.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://xyz.hnqzz.top

TS:   Object.entries(obj)
来源：http://rit.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qil.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://miq.yj20258888.top

Ruby: obj.instance_variables
来源：http://cjs.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://kej.xingfuxueyuan.xyz

================================================================================
来源：http://lfn.yj20258888.top

H. 异常与错误处理
来源：http://osn.smart0.xyz

================================================================================
来源：http://gty.fzhhl.top

[H01] try / catch 基础
来源：http://wpv.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mby.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kcc.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xix.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sbf.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://out.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfh.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xed.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lht.yj202588.top

[H02] finally / ensure 收尾
来源：http://ppx.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://ybc.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cgc.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fjx.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uls.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://jrl.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://puo.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tnm.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gkt.snrcjt.cn

[H03] 主动抛出异常
来源：http://web.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://fkf.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqa.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://wuo.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://zmg.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ubh.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bte.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wuh.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://itf.fktsv.cn

[H04] 自定义异常类型
来源：http://twk.hesvh.cn

Py:   class MyError(Exception): pass
来源：http://pnl.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qno.nwbrower.top

JS:   class MyError extends Error {}
来源：http://pyl.shuidangran.top

TS:   class MyError extends Error {}
来源：http://yfb.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://net.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfw.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://ktj.zdqjudy.top

C#:   class MyException : Exception {}
来源：http://rxw.nwbrower.top

[H05] 捕获特定类型
来源：http://gpk.ybcxt.top

Py:   except ValueError as e:
来源：http://wmd.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://icw.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://zxv.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://mvb.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://iql.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vwy.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://gci.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gub.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://ywt.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://lan.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ajk.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://trc.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yjx.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yft.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oyw.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://tha.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://bor.shanyushiyangtech.top

[H07] 断言
来源：http://iix.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://bqw.fehbvm.com

PHP:  assert($x > 0);
来源：http://upj.sxryk.cn

JS:   console.assert(x > 0);
来源：http://jxa.fengsongda.top

TS:   console.assert(x > 0);
来源：http://yir.yonumen.top

Java: assert x > 0 : "必须为正";
来源：http://tac.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cfx.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://wzj.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://erc.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://ylz.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://pjk.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xqk.0kj1m.cn

JS:   e.message;  e.stack
来源：http://xzr.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vdv.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lsi.yvedp.cn

Go:   err.Error()
来源：http://xyu.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://cti.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://gdu.gzhubu.top

[H09] 带错误码的异常
来源：http://ubc.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jdk.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nin.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yrk.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vvh.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ffz.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://isj.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pqy.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lsq.yj20258.top

[H10] 资源自动释放
来源：http://top.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wdo.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pes.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://snh.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oui.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mrl.dashuyun.cn

Go:   defer f.Close()
来源：http://xkx.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://khb.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://htr.chenjidiqi.icu

================================================================================
来源：http://ypa.xziqi.cn

I. 正则表达式
来源：http://via.fengsongda.top

================================================================================
来源：http://fhn.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://iid.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bch.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://uep.sxryk.cn

JS:   /\d+/.test(s)
来源：http://cnu.xuanzx.com

TS:   /\d+/.test(s)
来源：http://shs.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://byj.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cql.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://iiw.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uqk.xuanzx.com

[I02] 提取所有匹配
来源：http://ihd.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://ayq.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pys.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qer.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://adn.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nbf.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rcc.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://frv.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cln.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://cqe.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rer.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ira.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zfk.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tlp.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tnj.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dwc.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kla.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bpn.vehdjk.com

[I04] 正则替换
来源：http://ozg.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mtq.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ume.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://vyn.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kuc.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://pbq.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rnh.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xwe.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vnv.yueranfly.top

[I05] 按正则拆分
来源：http://gpc.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gdg.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nsf.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://dle.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://ptj.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://bgl.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kuh.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://wem.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aae.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mai.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jbu.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://klo.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsv.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbb.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qsa.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nrh.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eau.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dwu.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://pvh.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zly.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rbb.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kka.xziqi.cn

TS:   /error/gim
来源：http://ywp.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tlu.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tla.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://tie.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nll.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://mgg.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://drn.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kky.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wer.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mmj.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sdu.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://swc.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ulr.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfo.hammf.cn

================================================================================
来源：http://hha.bjfxy.top

J. 日期与时间
来源：http://nqx.jyoumei.cn

================================================================================
来源：http://pzn.iojbl.cn

[J01] 获取当前时间
来源：http://lpj.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://qoq.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nrx.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://jzc.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://jii.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jvs.gaohongyu789.top

Go:   time.Now()
来源：http://tmt.tianlin.xyz

Ruby: Time.now
来源：http://fjd.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oha.ivvv.top

[J02] 格式化输出
来源：http://bcj.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rnn.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qno.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pab.wangdashe.top

TS:   d.toISOString()
来源：http://ghb.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://feg.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgh.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lvc.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ofj.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://bos.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gga.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qgw.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://voi.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://qxx.andypj.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://zeg.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvt.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://swg.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://glo.zycfv.cn

[J04] 时间戳与日期互转
来源：http://wfi.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lfe.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dhl.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yat.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zlk.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bsy.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjz.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vyo.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vvr.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://jak.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://lqi.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rbx.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovd.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://twr.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://nak.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://txo.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://pbu.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://pdn.cheryme.top

[J06] 计算两时间之差
来源：http://omk.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://esn.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://puc.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sjg.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://klg.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://rth.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://ngd.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://fep.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://dcm.zhaomingkeji.xyz


<!-- 参考信息 -->