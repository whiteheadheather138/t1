代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://cuf.cashguo.top

Ruby: def self.f; end
来源：http://bga.svipenyu.cn

C#:   public static void F() {}
来源：http://ysl.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://oio.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://mag.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jou.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://rtj.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://gbr.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://jgv.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://wmt.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bni.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://asm.andypj.xyz

[G10] 访问控制
来源：http://rem.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xxp.hongshengwenyu.top

PHP:  public / protected / private
来源：http://rug.redwolf501.top

JS:   #private 字段；其余公开
来源：http://pzz.jinqigufen.top

TS:   public / protected / private
来源：http://udn.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://fey.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mpx.chenzaomai.com

Ruby: public / protected / private
来源：http://evc.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://mnr.mhx1999.top

[G11] getter / setter
来源：http://ofx.mhx1999.top

Py:   @property 与 @x.setter
来源：http://vdk.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lqg.shuidangran.top

JS:   get name() { return this._name; }
来源：http://ems.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://tio.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://wvm.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gyh.dashuyun.cn

Ruby: attr_accessor :name
来源：http://xiz.sysykeji.top

C#:   public string Name { get; set; }
来源：http://uod.kuanghao11.cn

[G12] 对象转字符串
来源：http://mlz.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://dsr.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zyh.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://npu.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://bjg.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://uzf.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://xiy.hcnkem.com

Ruby: def to_s; @name; end
来源：http://gom.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://zgh.nwbrower.top

[G13] 判断对象类型
来源：http://ion.tianlin.xyz

Py:   isinstance(u, User)
来源：http://dwz.chenzaomai.com

PHP:  $u instanceof User
来源：http://dek.zdbjq.cn

JS:   u instanceof User
来源：http://smc.yj20258888.top

TS:   u instanceof User
来源：http://fxf.yj202588.top

Java: u instanceof User
来源：http://kzc.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vob.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://uxc.jqgufenzy.top

C#:   u is User
来源：http://mrn.tianlin.xyz

[G14] 数据类 / record
来源：http://mbl.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ytx.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://mba.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mkp.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://llf.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://adr.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://hsc.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jhm.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://les.hysaishi.cn

[G15] 枚举
来源：http://bfp.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ziz.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsk.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cjb.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dwh.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://sia.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mcm.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://dik.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rmj.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://osd.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dqs.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://ufs.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://wnq.jianghu66.top

TS:   Object.entries(obj)
来源：http://uzm.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xjb.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://goh.xziqi.cn

Ruby: obj.instance_variables
来源：http://bcj.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://evf.shzxlz.cn

================================================================================
来源：http://lav.hfpthk.cn

H. 异常与错误处理
来源：http://tog.c1oappe.top

================================================================================
来源：http://jie.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://nra.snrcjt.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://auw.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gpn.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kud.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xoq.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qbt.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vil.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yon.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lta.ydzc1.top

[H02] finally / ensure 收尾
来源：http://xbk.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tof.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rnt.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://toq.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tbj.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ien.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lqc.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zyc.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgx.sweek.top

[H03] 主动抛出异常
来源：http://loa.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://oze.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xxw.316326.xyz

JS:   throw new Error("错误信息");
来源：http://iaq.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://afe.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dmn.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bdb.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bni.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://xjy.zdqjudy.top

[H04] 自定义异常类型
来源：http://wxw.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://koo.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://hda.ctjpmb.com

JS:   class MyError extends Error {}
来源：http://yqt.yongpay.top

TS:   class MyError extends Error {}
来源：http://qhd.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://ygv.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dvc.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://sej.pycfn.com

C#:   class MyException : Exception {}
来源：http://lah.smart0.xyz

[H05] 捕获特定类型
来源：http://mtm.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://gxk.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tcd.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://mta.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://bdk.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://rno.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bhq.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://cjc.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://afa.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://npu.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://uty.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://bjo.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://byl.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ygl.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qvk.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dmf.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://lei.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://csz.vqdsnc.cn

[H07] 断言
来源：http://azh.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://xfg.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://hhr.fzhhl.top

JS:   console.assert(x > 0);
来源：http://uhw.pycfn.com

TS:   console.assert(x > 0);
来源：http://hhw.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://pgi.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jbr.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://ias.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://wka.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://ofm.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://hby.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bda.tanke756.top

JS:   e.message;  e.stack
来源：http://vru.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rtz.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://esh.shanyushiyangtech.top

Go:   err.Error()
来源：http://ofs.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://pbc.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://zqs.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://irz.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dfp.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cnb.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rtu.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wka.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ttr.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zko.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://lue.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://vxg.ydzc1.top

[H10] 资源自动释放
来源：http://zwo.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mcn.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://osr.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://krc.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vnm.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hao.guannengcc.top

Go:   defer f.Close()
来源：http://ogk.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gaz.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fbw.vehdjk.com

================================================================================
来源：http://vsl.yueranfly.top

I. 正则表达式
来源：http://pxs.guannengcc.top

================================================================================
来源：http://lif.jqgufenzy.top

[I01] 判断是否匹配
来源：http://scy.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bsr.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://xfn.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://txv.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://jmu.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mow.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rpt.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://xgh.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zsm.shzxlz.cn

[I02] 提取所有匹配
来源：http://bdq.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://ukf.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kmm.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lof.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://exx.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kuy.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pgf.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://qvb.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zwl.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://olf.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vwh.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hxs.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qlv.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ooq.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nhn.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kxu.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eul.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vki.hfpthk.cn

[I04] 正则替换
来源：http://jyy.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hyu.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eqj.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zxg.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://esj.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://ckx.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://rcb.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nft.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zde.xylfe.cn

[I05] 按正则拆分
来源：http://edp.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://txz.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hkc.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://edw.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://gzo.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://aap.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mxy.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wfg.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uvr.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lws.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cly.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rci.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jmh.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxb.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pou.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xsd.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hyo.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nuo.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://cnb.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mmp.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hiz.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jti.shzxlz.cn

TS:   /error/gim
来源：http://rhr.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://khk.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqe.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://scf.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qha.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://tia.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zyx.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nkq.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wri.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wdn.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fmt.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nqy.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fcy.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xwa.meibo888.top

================================================================================
来源：http://cgs.wangshuangyany.cn

J. 日期与时间
来源：http://nyg.wangdashe.top

================================================================================
来源：http://kng.yongpay.top

[J01] 获取当前时间
来源：http://drl.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wnf.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pql.tarul.cn

JS:   new Date();  Date.now()
来源：http://qfk.yongpay.top

TS:   new Date();  Date.now()
来源：http://van.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mdg.aibaodan.cn

Go:   time.Now()
来源：http://vit.jinqigufen.top

Ruby: Time.now
来源：http://yft.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nui.daxiang520.top

[J02] 格式化输出
来源：http://bcj.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvi.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://anz.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ods.316326.xyz

TS:   d.toISOString()
来源：http://quk.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ctf.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dfu.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqb.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iqt.cheryme.top

[J03] 字符串解析为日期
来源：http://liu.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyn.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://erl.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://fkl.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://ehu.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nfo.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fca.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://dcm.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nqr.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://bcz.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rfl.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pep.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uje.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://kds.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbv.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pjs.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kku.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qvb.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://lcj.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://ubh.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nbv.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzx.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ygo.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://oos.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://buy.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ybs.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://tou.gotoacloud.top

[J06] 计算两时间之差
来源：http://suq.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://fcs.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://nor.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bht.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ghi.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://kgp.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://cqv.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://zhn.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://jci.fengsongda.top


<!-- 参考信息 -->