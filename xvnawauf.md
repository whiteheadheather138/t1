代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hou.hysaishi.cn

Ruby: def self.f; end
来源：http://njk.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://ism.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://ncy.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://ewl.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sfs.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oox.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://iqb.fengsongda.top

Java: interface Shape { double area(); }
来源：http://ffn.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://juy.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mlg.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://lfy.jinqigfzy.top

[G10] 访问控制
来源：http://ily.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://ffx.xziqi.cn

PHP:  public / protected / private
来源：http://oqp.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://oie.snrcjt.cn

TS:   public / protected / private
来源：http://tul.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://ytj.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cqz.chenzaomai.com

Ruby: public / protected / private
来源：http://cnt.daria6918.cn

C#:   public / protected / private / internal
来源：http://oyj.sufxvd.cn

[G11] getter / setter
来源：http://vca.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://xwt.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ylf.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://kfq.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://ohp.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://nmo.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zbu.sufxvd.cn

Ruby: attr_accessor :name
来源：http://xtc.daria6918.cn

C#:   public string Name { get; set; }
来源：http://dmi.sjlbkw.cn

[G12] 对象转字符串
来源：http://tvi.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://wrp.aibaodan.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://avr.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://dlk.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://tza.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://irn.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://piw.tian-w.cn

Ruby: def to_s; @name; end
来源：http://wyo.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://lpv.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://efh.hesvh.cn

Py:   isinstance(u, User)
来源：http://ilw.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://ddk.jianghu66.top

JS:   u instanceof User
来源：http://jjy.aizwys.cn

TS:   u instanceof User
来源：http://aaq.epnwcf.com

Java: u instanceof User
来源：http://blc.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bnb.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://yne.chenjidiqi.icu

C#:   u is User
来源：http://bgy.yangfankeji.com

[G14] 数据类 / record
来源：http://gtk.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uye.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://yfx.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://hsp.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://ogu.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://ovj.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://hjy.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kve.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://mnh.chenlongwang.top

[G15] 枚举
来源：http://ntp.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kfw.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bbr.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wan.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://thn.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://pwd.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kfj.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://yhj.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jqm.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://xxx.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bkb.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://fhe.shuidangran.top

JS:   Object.entries(obj)
来源：http://jhr.gzhubu.top

TS:   Object.entries(obj)
来源：http://fad.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dwk.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://udc.haohaochexian.top

Ruby: obj.instance_variables
来源：http://poj.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://huo.yj20258888.top

================================================================================
来源：http://vmu.zycfv.cn

H. 异常与错误处理
来源：http://nsq.hammf.cn

================================================================================
来源：http://kkc.hesvh.cn

[H01] try / catch 基础
来源：http://bvh.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wpt.yuxming.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://twg.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://znk.nwbrower.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cil.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ufa.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tcg.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uvh.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jre.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://obw.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://die.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vzr.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mbz.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gok.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://uao.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hfa.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://kxc.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uwt.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://pxk.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://jww.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rrc.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://umx.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://dit.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jvm.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wln.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://etq.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vsw.vqdsnc.cn

[H04] 自定义异常类型
来源：http://azb.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://gzh.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ehr.hammf.cn

JS:   class MyError extends Error {}
来源：http://tzm.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://grn.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://aev.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rge.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://uzx.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://sse.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://ore.bjfxy.top

Py:   except ValueError as e:
来源：http://vcc.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oct.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://gow.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://osm.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://vut.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ohr.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://hfu.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfo.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://wle.tianlin.xyz

Py:   value = d.get("k") or default
来源：http://pzj.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lfw.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hol.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hjz.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zse.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://agi.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://bgb.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://ueu.shuidangran.top

[H07] 断言
来源：http://nps.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://iss.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://pwx.yonumen.top

JS:   console.assert(x > 0);
来源：http://lsr.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://cbu.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://ojc.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cra.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://cng.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://avs.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://kck.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://cwk.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rvj.ybcxt.top

JS:   e.message;  e.stack
来源：http://zdp.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://lyt.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vtt.jiagoushi.top

Go:   err.Error()
来源：http://ipk.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://xmz.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://oiu.zhoulong.xyz

[H09] 带错误码的异常
来源：http://lqg.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nxn.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xre.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sze.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xyr.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xwk.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://irl.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://xme.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wyz.dashuyun.cn

[H10] 资源自动释放
来源：http://img.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://lza.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rgb.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xzr.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://apl.wangshuangyany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://izx.fzhhl.top

Go:   defer f.Close()
来源：http://hof.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xor.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vys.pycfn.com

================================================================================
来源：http://nfx.hnqzz.top

I. 正则表达式
来源：http://wmk.wangshuangyany.cn

================================================================================
来源：http://guc.hfpthk.cn

[I01] 判断是否匹配
来源：http://njz.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nvh.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://pcj.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://fhv.andypj.xyz

TS:   /\d+/.test(s)
来源：http://ipw.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ids.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pye.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://zpv.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjt.zdbjq.cn

[I02] 提取所有匹配
来源：http://eww.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://vdk.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pwj.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://upc.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://zlg.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zja.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rzf.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://ebi.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rwl.birdmap.top

[I03] 提取捕获分组
来源：http://fqa.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tzg.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqd.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fci.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vyr.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xxj.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpt.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sec.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gqb.xuanzx.com

[I04] 正则替换
来源：http://kfv.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cab.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ine.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://qye.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://cnb.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wgm.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wmc.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sxo.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bpk.redwolf501.top

[I05] 按正则拆分
来源：http://bbr.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iht.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exg.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://wgh.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://ujl.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://emc.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wof.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://gkl.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vwe.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wgi.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xhw.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qbk.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tbi.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://coq.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://duz.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsl.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uua.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ofj.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://wza.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rqr.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ipw.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qga.yanxiufei.cn

TS:   /error/gim
来源：http://bui.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lvy.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bpp.ybcxt.top

Ruby: s.scan(/error/i)
来源：http://hup.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://epl.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://xwj.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tmn.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rjg.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uom.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uqe.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ciu.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ypf.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://itg.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ebt.zhongyouzk.top

================================================================================
来源：http://nfr.yuxming.cn

J. 日期与时间
来源：http://okq.gaohongyu789.top

================================================================================
来源：http://und.svipenyu.cn

[J01] 获取当前时间
来源：http://iec.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thw.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://onl.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://dpm.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://adj.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://pbc.nwbrower.top

Go:   time.Now()
来源：http://hgw.yvedp.cn

Ruby: Time.now
来源：http://dea.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hbz.shangyingyoupin.top

[J02] 格式化输出
来源：http://xbm.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lcw.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oml.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lyx.wangshuangyany.cn

TS:   d.toISOString()
来源：http://ssv.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kca.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fxj.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oki.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hqm.ctjpmb.com

[J03] 字符串解析为日期
来源：http://sfs.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aoc.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kbx.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://mvs.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://llf.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://crx.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ryy.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://ucx.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fut.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://cbn.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wjb.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sml.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://prh.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jem.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lbh.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vll.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fzz.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://neb.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://pba.havefunace.top

Py:   now + timedelta(days=7)
来源：http://bkq.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hyr.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxt.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ynl.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://qxf.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ols.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://oze.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://isk.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://kvx.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://nsg.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://mzq.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://acg.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xun.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://yus.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://ufs.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://dft.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://kac.tianlin.xyz


<!-- 参考信息 -->