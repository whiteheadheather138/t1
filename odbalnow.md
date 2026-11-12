代发 wailian999

PHP:  public static function f() {}
来源：http://jfb.ivvv.top

JS:   static f() {}
来源：http://ixe.zycfv.cn

TS:   static f(): void {}
来源：http://iax.fzhhl.top

Java: static void f() {}
来源：http://qyf.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wzo.aizwys.cn

Ruby: def self.f; end
来源：http://aoh.sufxvd.cn

C#:   public static void F() {}
来源：http://eib.bjfxy.top

[G09] 接口 / 抽象类
来源：http://unt.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://yma.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://kjh.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bgx.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://riv.yj202588.top

Java: interface Shape { double area(); }
来源：http://lib.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://jbd.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hzs.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://cnq.vehdjk.com

[G10] 访问控制
来源：http://jef.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://yus.gogol.net.cn

PHP:  public / protected / private
来源：http://dhi.xylfe.cn

JS:   #private 字段；其余公开
来源：http://tnv.zhixingplan.top

TS:   public / protected / private
来源：http://cgk.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://vxf.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uyn.daxiang520.top

Ruby: public / protected / private
来源：http://qtp.nanxinkj.top

C#:   public / protected / private / internal
来源：http://qeh.52xcode.cn

[G11] getter / setter
来源：http://txo.jianghu66.top

Py:   @property 与 @x.setter
来源：http://rug.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fxf.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://yxm.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://dax.hcnkem.com

Java: public String getName() { return name; }
来源：http://cpv.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sre.tian-w.cn

Ruby: attr_accessor :name
来源：http://tzh.bbcook.cn

C#:   public string Name { get; set; }
来源：http://ndp.snrcjt.cn

[G12] 对象转字符串
来源：http://kwz.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://ios.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xjr.fehbvm.com

JS:   toString() { return this.name; }
来源：http://ihx.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://tkj.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://ofe.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://dhp.iojbl.cn

Ruby: def to_s; @name; end
来源：http://pik.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://gvs.wangdashe.top

[G13] 判断对象类型
来源：http://vdi.zdqjudy.top

Py:   isinstance(u, User)
来源：http://rag.yj202588.top

PHP:  $u instanceof User
来源：http://uor.feifeiyinyue.top

JS:   u instanceof User
来源：http://vty.ydzc1.top

TS:   u instanceof User
来源：http://qrd.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://fls.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://guh.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://seo.hnqzz.top

C#:   u is User
来源：http://vqd.vqdsnc.cn

[G14] 数据类 / record
来源：http://oce.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ong.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://cxv.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://yze.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://ghm.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://ohe.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://mfv.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mco.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://ccf.hysaishi.cn

[G15] 枚举
来源：http://anh.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kuv.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qoe.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://flq.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://boh.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://xrp.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uru.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://xxk.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofk.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://jtw.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hpk.guannengcc.top

PHP:  get_object_vars($obj);
来源：http://mdo.zhengqikj.top

JS:   Object.entries(obj)
来源：http://vdw.shzxlz.cn

TS:   Object.entries(obj)
来源：http://prn.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hnf.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cwz.yuxming.cn

Ruby: obj.instance_variables
来源：http://dhb.jqgfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://rfi.chenjidiqi.icu

================================================================================
来源：http://lwc.zhoulong.xyz

H. 异常与错误处理
来源：http://gdh.yfazqb.com

================================================================================
来源：http://qpz.smart0.xyz

[H01] try / catch 基础
来源：http://buj.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zkw.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hva.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tcb.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kbk.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://roj.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://brl.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ycn.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ars.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://pio.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://btc.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yve.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://drz.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cpa.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://jzn.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbh.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kvb.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uab.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://khn.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://uos.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://usq.havefunace.top

JS:   throw new Error("错误信息");
来源：http://vfk.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://ntd.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lpu.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://onn.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tad.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://zdh.dashuyun.cn

[H04] 自定义异常类型
来源：http://qql.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://rsv.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vfl.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://pzw.xylfe.cn

TS:   class MyError extends Error {}
来源：http://xai.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://pkw.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zvt.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://hdf.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://bgz.hesvh.cn

[H05] 捕获特定类型
来源：http://knp.tian-w.cn

Py:   except ValueError as e:
来源：http://qct.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cuz.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://zgc.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://ssb.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://afp.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ipf.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://zmw.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iif.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://zkp.52xcode.cn

Py:   value = d.get("k") or default
来源：http://stf.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://koo.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ilh.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://sbn.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nnp.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xpp.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://kqt.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://sms.jqgfzy.top

[H07] 断言
来源：http://ype.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://uby.yj20258.top

PHP:  assert($x > 0);
来源：http://uea.meibo888.top

JS:   console.assert(x > 0);
来源：http://pxo.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://vgr.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://hhz.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vyh.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hrk.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://swt.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://oso.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://icd.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjd.yfazqb.com

JS:   e.message;  e.stack
来源：http://nbx.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rye.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lxb.quarkkingdee.top

Go:   err.Error()
来源：http://ugz.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://xfu.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://pso.hfpthk.cn

[H09] 带错误码的异常
来源：http://nly.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://chd.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fng.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jns.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fwl.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pst.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nqg.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://tcx.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dau.jyoumei.cn

[H10] 资源自动释放
来源：http://ctk.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://wqr.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ldt.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pdu.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oqp.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://las.andypj.xyz

Go:   defer f.Close()
来源：http://wdk.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hiq.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zul.vqdsnc.cn

================================================================================
来源：http://gkx.nwbrower.top

I. 正则表达式
来源：http://kva.zhoulong.xyz

================================================================================
来源：http://pwd.zhengqikj.top

[I01] 判断是否匹配
来源：http://pvs.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcl.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jtk.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://peu.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://thy.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fad.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uzt.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://isk.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dqf.wangdashe.top

[I02] 提取所有匹配
来源：http://loa.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://eqc.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvp.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gtp.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://tmt.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://atb.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://efx.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://vah.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wkr.sweek.top

[I03] 提取捕获分组
来源：http://kzy.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xdr.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ptc.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kic.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yuc.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mdb.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pfa.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xmv.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fad.xuanzx.com

[I04] 正则替换
来源：http://vgj.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sdj.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pdg.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://gcz.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://ucp.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ziy.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fyp.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zjr.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pgh.zhijiandao.cn

[I05] 按正则拆分
来源：http://bpr.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tco.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vug.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://smr.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://vhb.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://eln.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ott.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://gbu.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rgo.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lfa.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ncj.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fml.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxu.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tul.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oto.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yzr.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zte.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jcw.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://iez.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qdf.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tgj.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mcf.hfpthk.cn

TS:   /error/gim
来源：http://ghj.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dpq.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://syx.havefunace.top

Ruby: s.scan(/error/i)
来源：http://pgp.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ahz.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://llf.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iey.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dgh.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eku.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://foz.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gnc.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jns.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://axz.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://itm.uphjek.com

================================================================================
来源：http://yxe.tian-w.cn

J. 日期与时间
来源：http://sya.jqgfzy.top

================================================================================
来源：http://etd.ydjk.org.cn

[J01] 获取当前时间
来源：http://bgk.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zuw.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://urj.cucudq.cn

JS:   new Date();  Date.now()
来源：http://jqg.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://dtf.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://awd.guannengcc.top

Go:   time.Now()
来源：http://ygf.yfazqb.com

Ruby: Time.now
来源：http://bpt.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zao.hnqzz.top

[J02] 格式化输出
来源：http://dum.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lzr.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zgm.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://btx.ydzc1.top

TS:   d.toISOString()
来源：http://hbc.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tuv.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rvr.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://arm.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://toe.zhengqikj.top

[J03] 字符串解析为日期
来源：http://doj.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nga.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aou.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://lbi.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://mic.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dkt.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dwq.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://oky.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://edm.c1oappe.top

[J04] 时间戳与日期互转
来源：http://ikh.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zxx.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tog.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cxx.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hhe.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ucp.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tlt.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gqe.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yva.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://pag.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://bdr.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fjj.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://psx.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xus.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://bhp.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rlk.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://nzj.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://adh.ydzc1.top

[J06] 计算两时间之差
来源：http://bvx.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://cny.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://gmn.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fas.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oym.cucudq.cn


<!-- 参考信息 -->